# Mission 4 Reflection

This laboratory activity helped me understand how containerization can be used in cloud computing and how Docker differs from traditional Virtual Machines. One of the most noticeable differences is the boot time and setup process. A Virtual Machine normally requires a complete operating system to be installed and started, which can take more time and consume more resources. In comparison, a Docker container uses an existing host operating system kernel and can start very quickly. In this activity, I was able to deploy an Nginx web server using only a few Docker commands.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80. The mapping connects port 8080 on the host environment to port 80 inside the container. This allowed me to access the Nginx server by using `curl http://localhost:8080`. Without the port mapping, the service inside the container would not be directly accessible through the host's port 8080.

I also learned that `docker rm` removes a container after it has been stopped. Any data stored only inside the container's writable layer can be lost when the container is removed. This shows why persistent data should be stored using appropriate Docker storage mechanisms when data needs to survive the container lifecycle.

Containerization can also improve collaboration between software developers and IT operations teams. Developers can package an application with its dependencies, while operations teams can deploy the same containerized application in a consistent environment. This supports DevOps practices by making deployment and management more predictable.

Finally, my GitHub portfolio is evolving by adding another practical laboratory project. Instead of only documenting concepts, I am now including actual Docker commands, screenshots, Markdown documentation, and evidence of a working containerized web server.

