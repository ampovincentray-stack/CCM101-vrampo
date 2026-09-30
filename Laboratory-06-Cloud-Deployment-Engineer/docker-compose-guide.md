# Docker Compose Guide

## What Does the `services:` Block Do?

The services block comprises the various services or containers that constitute an application. In this lab activity, it contains two services namely: database and app. The database service is based on MariaDB 10.6 and the app service is based on the Nextcloud image. Docker Compose uses these specifications to create and maintain the containers together.

## How Does the Nextcloud App Container Find the Database?

Nextcloud’s software detects your DB using the MYSQL_HOST environment variable. Our docker-compose.yml has the line MYSQL_HOST=database — this means that we connect nextcloud to a service called “database”.

Due to the way internal network and DNS are handled within docker compose, you don’t need to specify an ip address, as nextcloud will automatically resolve the name to the appropriate server (in our case a mariadb container).

## Difference Between `docker run` and `docker-compose up -d`

In short, when you use the docker run command, you are creating and starting an individual container with some configuration that you specify using the command line options.

On the other hand, using the docker compose up -d will let you create and start several connected containers at once by providing the configuration details in a YAML format configuration file. Also, the –d (or --detach) option starts all those containers on the background. So you can get back to your terminal to do other things.

## Conclusion

With Docker Compose you’ll be able to easily deploy and manage your multi container applications by using this YAML file which will have all the configurations needed for deploying and managing your related service’s.
