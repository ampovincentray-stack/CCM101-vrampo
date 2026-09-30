# Laboratory 06 – The Cloud Deployment Engineer

## Mission Overview

The goal of this lab is to deploy a multi-tier cloud application (web app + DB) based on Nextcloud and MariaDB through the use of Docker-Compose.
Both services are declared inside a “docker-compose.yml” file.

## Objectives

* Explain the concept of a two-tier application architecture.
* Understand the purpose and structure of a `docker-compose.yml` file.
* Use the Nano text editor to create a configuration file.
* Deploy a multi-container application using Docker Compose.
* Access the Nextcloud installation page through a browser.
* Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown.
* Expand the GitHub Cloud Computing Portfolio.

## Commands Executed

| Command                      | Description                                           |
| ---------------------------- | ----------------------------------------------------- |
| `mkdir nextcloud-deployment` | Creates the project directory.                        |
| `cd nextcloud-deployment`    | Enters the project directory.                         |
| `nano docker-compose.yml`    | Creates or edits the Compose configuration.           |
| `cat docker-compose.yml`     | Displays the configuration file.                      |
| `docker-compose up -d`       | Starts the application stack in the background.       |
| `docker-compose ps`          | Checks the status of the containers.                  |
| `docker-compose logs`        | Displays container logs.                              |
| `docker-compose down`        | Stops and removes the Compose containers and network. |

## Skills Learned

* Understanding two-tier architecture.
* Writing YAML configuration files.
* Using the Nano text editor in Linux.
* Deploying and managing containers with Docker Compose.
* Configuring communication between containers.
* Accessing a web application through a mapped port.
* Applying Infrastructure as Code principles.
* Documenting technical work using Markdown and GitHub.

## Screenshots

The screenshots for this laboratory activity are available in the `screenshots/` folder.

* `compose-deployment.png`
* `nextcloud-web.png`
* `compose-teardown.png`

