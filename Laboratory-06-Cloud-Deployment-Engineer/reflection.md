# Mission Reflection

In this Laboratory Activity 6, I learned how to deploy a multi-container application using Docker Compose. Before doing this activity, I understood that Docker could run individual containers, but I did not fully understand how multiple containers could work together. Through this activity, I learned how Nextcloud and MariaDB communicate with each other to provide a private cloud storage system.

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows multiple containers to be configured and deployed using a single file. Instead of manually typing many commands for each container, we can define the services and their settings in one configuration. This also makes deployment more organized and repeatable.

I also learned that YAML indentation is very important. If I accidentally use a Tab instead of spaces or place a line at the wrong indentation level, Docker Compose may fail to read the configuration correctly. This can prevent the application from starting, so it is important to check the formatting carefully.

Environment variables, such as `MYSQL_PASSWORD` and `MYSQL_DATABASE`, allow the containers to use the required database settings. They make the configuration easier to manage and help the Nextcloud application connect to MariaDB.

Deploying Nextcloud using Docker Compose helped me understand how cloud applications can be set up with only a few commands. It was interesting to see how the application and database work together in separate containers. However, I also learned that successful deployment requires proper configuration and verification.

Since Mission 1, my understanding of cloud computing has improved. I now understand more about containers, application architecture, and Infrastructure as Code. This activity helped me appreciate how automation can simplify the deployment and management of cloud applications.

