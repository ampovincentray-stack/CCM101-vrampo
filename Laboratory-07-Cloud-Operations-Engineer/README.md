# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on cloud operations, Linux system monitoring, Docker container deployment, application logging, and real-time performance monitoring. Using the KillerCoda Playground, I performed a baseline health check, deployed an Nginx web server, generated HTTP requests, and examined the resulting logs and container metrics.

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

Through this activity, I practiced Linux resource monitoring, Docker deployment, HTTP request testing, log analysis, performance observation, Markdown documentation, and GitHub portfolio management.

## Repository Contents

* `system-baseline-report.md` — Host resource baseline.
* `container-observability.md` — Application logs and container metrics.
* `reflection.md` — Personal learning reflection.
* `screenshots/` — Terminal evidence for the checkpoints.

