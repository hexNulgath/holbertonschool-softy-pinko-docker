# Use the latest Ubuntu base image
FROM ubuntu:latest

# Set the working directory to /app
WORKDIR /app

# Update APT, upgrade all software, install Python3, pip3, and Flask
RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y python3 python3-pip && \
    rm /usr/lib/python*/EXTERNALLY-MANAGED && \
    pip3 install Flask

# Copy the Flask application into the container
COPY api.py /app/api.py

# Expose port 5252 to allow traffic to the Flask app
EXPOSE 5252

# Command to run the Flask app
CMD ["python3", "api.py"]
