FROM ubuntu:latest

# Update and upgrade system
RUN apt-get update && apt-get upgrade -y

# Install Python and pip
RUN apt-get install -y python3 python3-pip

# Fix "externally managed environment" issue
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy Flask app into container
COPY api.py /app/api.py

# Expose Flask port
EXPOSE 5252

# Run the Flask app
CMD ["python3", "api.py"]
