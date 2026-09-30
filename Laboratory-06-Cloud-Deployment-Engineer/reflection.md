# Mission Reflection

In Laboratory Activity 6, I learned to deploy a multi-container app with Docker Compose. Before participating in this activity, I had knowledge of Docker being capable of running single containers but I was not quite familiar with working with multiple containers. This was uncovered through this activity where I learned that Nextcloud and MariaDB communicate with each other in order to set up a private cloud storage system.

Preparing a docker-compose.yml file comes in handy for a cloud engineer because it allows configuring and deploying multiple containers in one file. Instead of running numerous commands for each of the containers, we are able to specify all the services and settings in one configuration.

I found that indentation in YAML is critical because if I mistakenly leave out spaces and put a Tab character or an additional space on a line, Docker Compose won’t be able to read the configuration properly. That could prevent the application from starting, and it is very important to follow the formatting rules precisely.

When working with containers, one should keep in mind that the environment variables, for example MYSQL_PASSWORD and MYSQL_DATABASE, can enable the containers to work with the required database settings properly. Using those variables makes the configuration easier to manage and provides Nextcloud with the ability to connect to the MariaDB database.

Deploying Nextcloud on a Docker Compose environment has given me an insight into the way a cloud application can be created with a few commands. I learned that it is interesting to see how the application and database function together in multiple containers but also that one needs to do proper configuration and validation of the process for it to be successful.

After completing Mission 1, I gained insight into the cloud computing field. The understanding I have around containers has increased. In addition to this, my knowledge of software architecture and Infrastructure as Code has improved simultaneously. The task provided me with the information regarding the power of automation as it can ease deployment and management of applications.
