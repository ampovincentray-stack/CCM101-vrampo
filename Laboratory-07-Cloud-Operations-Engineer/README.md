# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

In this lab, cloud computing operations, Linux based server monitoring, deployment of Docker containers, and logging and monitoring of applications were covered as well as logging and monitoring of application performance were dealt with. I utilized the KillerCoda Playground to conduct a baseline evaluation, deploy an Nginx web server, generate HTTP requests, and analyze the metrics and logs of the container.


## Objectives

* Monitor Linux host memory and disk capacity.
* Observe CPU utilization and active processes.
* Deploy an Nginx container named `client-website`.
* Generate successful HTTP requests and an intentional HTTP 404 error.
* Analyze application access logs.
* Monitor CPU, memory, and network activity with Docker.
* Document the results and maintain a GitHub Cloud Computing portfolio.

## Monitoring Commands Executed

| Command                                                | Purpose                                     |
| ------------------------------------------------------ | ------------------------------------------- |
| `free -h`                                              | Check memory usage.                         |
| `df -h /`                                              | Check root filesystem capacity.             |
| `top`                                                  | Observe CPU activity and running processes. |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx container.                 |
| `docker ps`                                            | Check running containers.                   |
| `curl`                                                 | Generate HTTP requests.                     |
| `docker logs client-website`                           | Inspect application logs.                   |
| `docker stats`                                         | Monitor live container metrics.             |

## Skills Learned

This lab enabled me to practice Linux resource monitoring, deployment of Docker containers, testing and analysis of HTTP requests as well as logging, monitoring, and Markdown documentation.

## Repository Contents

* `system-baseline-report.md` — Host resource baseline.
* `container-observability.md` — Application logs and container metrics.
* `reflection.md` — Personal learning reflection.
* `screenshots/` — Terminal evidence for the checkpoints.

