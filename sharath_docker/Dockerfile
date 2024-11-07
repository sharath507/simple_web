# FROM python:3.9-slim

# WORKDIR /app

# COPY . /app

# RUN pip install requests

# CMD ["python","app.py"]

# -------------------------------------------
# FROM python:3.8-slim


# # FROM nginx:alpine

# WORKDIR /app

# COPY requirements.txt .
# RUN pip install --no-cache-dir -r requirements.txt

# COPY . .

# CMD ["python", "app.py"]

# EXPOSE 5000



# Use an official Python runtime as a base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Set environment variables
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0

# Expose the port that the app will run on
EXPOSE 5000

# Run the application
# CMD ["flask", "run"]
CMD ["python","app.py"]

