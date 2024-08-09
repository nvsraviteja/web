# Use the official Python image from the Docker Hub
FROM python:3.9

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy requirements file to the container
COPY requirements.txt ./

# Install the Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code to the container
COPY . /usr/src/app/src/

# Expose the port that the application will run on
EXPOSE 8000

# Define the command to run the application
CMD ["python", "Flask/app.py"]

