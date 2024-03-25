# Use an official Python runtime as the base image
FROM python:3.9-slim

# Copy requirements.txt from build context first 
COPY requirements.txt .

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Set the working directory in the container
WORKDIR /app

# Copy project
COPY .. /app

# Make port 8888 available to the world outside this container
EXPOSE 8888