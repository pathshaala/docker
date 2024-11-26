# Use an official Alpine image for a minimal container
FROM alpine:latest

# Install ping utility (part of iputils)
RUN apk add --no-cache iputils

# Set the default command to ping Google
ENTRYPOINT ["ping", "-c", "5"]

# Set the default target to google.com
CMD ["google.com"]
