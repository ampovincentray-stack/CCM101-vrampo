# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

This laboratory activity introduces cloud-native technologies, especially containers and Docker. The activity focuses on understanding the differences between traditional Virtual Machines and containers and deploying an Nginx web server using Docker.

## Objectives

* Differentiate between Virtual Machines and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate an Nginx container.
* Document container operations using Markdown.
* Continue developing the GitHub Cloud Computing portfolio.

## Docker Commands Executed

The following Docker commands were used during this laboratory:

```bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
```

## Skills Learned

Through this activity, I learned how to verify a Docker environment, download a Docker image, create and run a container, map a network port, test a web server, and manage the container lifecycle.

## Challenges Encountered

One challenge was understanding the difference between a Docker image and a running container. I also had to make sure that the correct port was mapped so that the Nginx web server could be accessed through port 8080. Reading the terminal output and executing the commands step by step helped me understand how Docker manages applications.

