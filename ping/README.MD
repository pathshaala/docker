Here’s a `README.md` file based on the information you provided, with additional details to help others understand how to use the Docker image:

---

# Ping Docker Image

This Docker image allows you to ping a specified domain or the default Google DNS (8.8.8.8) if no domain is provided.

### Default Behavior
When no domain is provided, it will ping google.com by default.

### Usage

1. **Ping Google DNS (default):**
   ```bash
   docker run bhavyabapna/ping
   ```
   This will run the container and ping `google.com`.

2. **Ping a specific domain (e.g., github.com):**
   ```bash
   docker run bhavyabapna/ping github.com
   ```
   This will run the container and ping `github.com`.

### Example

- **Default Ping (Google DNS):**
   ```bash
   docker run bhavyabapna/ping
   ```
   Output:
   ```bash
   Pinging google.com...
   ```

- **Ping GitHub:**
   ```bash
   docker run bhavyabapna/ping github.com
   ```
   Output:
   ```bash
   Pinging github.com...
   ```


### Notes:
- If you provide a domain (e.g., `docker run bhavyabapna/ping github.com`), it will override the default and ping the provided domain.
- The image uses `ping` from `iputils` which is a lightweight package in Alpine Linux.
