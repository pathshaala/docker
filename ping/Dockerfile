# Use an official Alpine image for a minimal container
FROM alpine:latest

# Install ping utility (part of iputils)
RUN apk add --no-cache iputils

# Set the default command to ping Google
CMD [ "google.com" ]
ENTRYPOINT [ "ping","-c","5" ]