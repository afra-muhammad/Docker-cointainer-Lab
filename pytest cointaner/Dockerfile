# Use the official Python slim image as the base image
FROM python:3.9-slim

# Meta-data about the container
LABEL maintainer="Afra Muhammad afra.muhammad@edu.dsti.institute" \
      description="Docker Pytest Workflow: Setting up an environment for running unit tests using Pytest."

# Set the working directory inside the container
WORKDIR /app

# Install pytest and any other required libraries
RUN pip install pytest

# Copy the current directory contents into the container at /app
COPY . .

# Create a mount point for external files
VOLUME /app

# Default command to run when the container launches (execute pytest)
CMD ["pytest"]

