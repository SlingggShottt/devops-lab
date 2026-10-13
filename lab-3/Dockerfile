# Created by Divyansh on 13 October 2026

# Base image
FROM python

# main working directory
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the app code
COPY . .

# Set environment variables
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
ENV FLASK_RUN_PORT=10001

# Set the port 
EXPOSE 10001

# Command to run the application
CMD ["flask", "run"]