# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the different services or containers that make up an application. In this laboratory activity, it contains two services: `database` and `app`. The `database` service uses MariaDB 10.6, while the `app` service uses the Nextcloud image. Docker Compose uses these definitions to create and manage the containers together.

## How Does the Nextcloud App Container Find the Database?

The Nextcloud application finds the database through the `MYSQL_HOST` environment variable. In our Docker Compose file, `MYSQL_HOST=database` tells Nextcloud to connect to the service named `database`. Docker Compose provides internal networking and service-name resolution, allowing the Nextcloud container to communicate with the MariaDB container without requiring its IP address.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is used to create and start an individual container by specifying its configuration through command-line options. In contrast, `docker-compose up -d` uses a YAML configuration file to create and start multiple related containers together. The `-d` option runs the containers in the background, allowing the terminal to be used for other tasks.

## Conclusion

Docker Compose makes it easier to deploy and manage a multi-container application. By defining the application in a YAML file, cloud engineers can use a repeatable configuration to start and manage related services.

