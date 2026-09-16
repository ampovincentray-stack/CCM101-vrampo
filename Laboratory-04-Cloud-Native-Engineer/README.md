# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

In this lab, students will explore cloud-native technologies, namely containers and Docker. The objective of this laboratory activity is to gain insight into the distinctions between conventional virtual machines and containers and deploy an Nginx Web Server using Docker.

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

Because of this activity, I learned how to verify a Docker environment, download a Docker image, create and run a container, map a network port, test a web server, and use the container lifecycle.

## Challenges Encountered

I formerly struggled with the difference between a docker image and a container in how they work. I also needed to check if I had properly mapped the port to connect to the Nginx web server identified through port 8080. In this regard, following the terminal messages and executing the commands made me understand how Docker works with different applications.
