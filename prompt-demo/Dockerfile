# Use a base image with Bash (e.g., Alpine or Ubuntu)
FROM ubuntu:latest

# Set the working directory inside the container
WORKDIR /app

# Copy the script to the container
COPY prompt.sh .

# Make the script executable
RUN chmod +x prompt.sh

# Run the script by default
CMD ["./prompt.sh"]
