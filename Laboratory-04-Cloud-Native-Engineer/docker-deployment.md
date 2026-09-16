# Docker Deployment

## Docker Environment

The Docker environment was verified using the following commands:

```bash
docker --version
docker info
```

### docker --version

This command displays the installed Docker version.

### docker info

This command displays information about the Docker environment and confirms that the Docker service is available.

## Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub so that it can be used to create a container.

## Run the Nginx Container

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```

This command creates and starts an Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

## Test the Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx server through port 8080 and verifies that the Nginx welcome page is running.

## Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command displays the containers that are currently running.

### 2. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 3. Verify the Container Is Stopped

```bash
docker ps
```

This command confirms that the stopped Nginx container is no longer listed among the running containers.

To also view stopped containers:

```bash
docker ps -a
```

### 4. Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped Nginx container from the Docker environment.

