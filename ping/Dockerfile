# Use an official Alpine image for a minimal container
FROM ubuntu:latest

# Install ping utility (part of iputils)
RUN apt install -y iputils-ping

# Set the default command to ping Google
ENTRYPOINT ["ping","-c","5"]

# Set the default target to google.com
CMD ["google.com"]
