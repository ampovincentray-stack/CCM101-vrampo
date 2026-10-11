# Laboratory Activity 7 Reflection

The laboratory activity helped me identify that monitoring is an essential component of cloud application management. For an application to function correctly, it is not sufficient to only place a container on a host server. There must be adequate resources on the host server. If the host server is lacking RAM, or have a high CPU load, or have inadequate disk space, for example, this will definitely impact the performance and the functionality of the application. Resource verification is therefore a useful exercise to help address potential situations that could lead to application failure.

I learned that docker logs are very useful for debugging. User login issues with the web app, for instance, can be found in logs, along with a request ID and other messages pertaining to the issue. So logs can definitely provide some useful information, but they can’t always provide all the information pertaining to a case.

Another lesson learned is the difference between metrics and logs. Logs register individual events e.g. whether a request was successful or not, or whether an HTTP server error has occurred. On the contrary, metrics provide a number of measurements i.e. CPU load, memory, and network activity.  Their combination allows obtaining a deeper understanding of an application health: logs provide information about what happened, while metrics measure performance.

In big enterprise companies, it can be hard to check on thousands of containers manually. Software products like Prometheus can be used to gather and store metrics data while Grafana allows monitoring through display of dashboards.

In summary, this activity enhanced my Linux commands and Docker monitoring tools. It also aided in checking system resources, deploying Nginx, creating and managing HTTP requests and accessing and understanding access logs. I also learned to capture screenshots and document the real outcomes of commands I run. These helped understand how cloud operations engineers use tangible pieces of information to investigate and continue providing a service that the end user has come to rely on.
