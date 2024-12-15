# Basic-HTTP-Server

##**Basic Usage**
``` bash
docker pull dogukaneren/basic-http-server
```

``` bash
docker run dogukaneren/basic-http-server
```


## **Dockerfile Usage and Setup**

1. Navigate to the directory containing the Dockerfile:
   ```bash
   cd Docker
   ```

2. Build the Docker image:
   ```bash
   docker build -t basic-http-server .
   ```

   Once the process is complete, a message like the following will appear with the image ID:
   ```
   Successfully built e2503c3799a4
   ```

## **Running the Server**

3. Start the Docker container:
   ```bash
   docker run -p 80:80 basic-http-server
   ```

   This command starts the HTTP server on the default port **80**.

## **Running with a Custom Port**

If you want to use a different port, you can specify it using an environment variable as follows:

```bash
docker run -e PORT=<your-port> -p <host-port>:<container-port> basic-http-server
```

### Example:
```bash
docker run -e PORT=8080 -p 8080:8080 basic-http-server
```

This command runs the server on port 8080.
