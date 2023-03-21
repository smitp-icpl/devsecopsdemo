# Use the official Python image as the base image
FROM python:3.10.10-slim-buster
# Set the working directory in the container
WORKDIR /app
# Copy the application code into the container
COPY . .

# Install the dependencies for the application
RUN pip install --no-cache-dir -r requirements.txt
#RUN pip install -r requirements.txt

# Expose the port that the application listens on
EXPOSE 5000
# Start the application
CMD ["python", "app.py"]