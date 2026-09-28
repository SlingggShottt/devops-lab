# Created by Divyansh on 29 september 2026

# Base image
FROM python:3.9-slim

# main workig directory
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the app code
COPY . .

# Set environment variables
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
ENV FLASK_RUN_PORT=5000

# Set the port 
EXPOSE 5000

# Command to run the application
CMD ["flask", "run"]