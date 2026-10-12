# Container Observability Report

## 1. Application Logs

**Command executed:** `docker logs client-website`

### HTTP 404 Error Log

172.17.0.1 [11/Oct/2026:19:15:15 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0"

2026/10/11 19:15:15 [error] 29#29: *4 open() "/usr/share/nginx/html/hidden-admin-page" failed (2: No s uch file or directory), client: 172.17.0.1, server: localhost, request: "GET /hidden-admin-page HTTP/1 .1", host: "localhost:8080"

### Why Application Logs Are Important

Logs capture actions taken, display errors, and contain other information that is often valuable during the debugging process. Engineers are often able to identify which requests failed and include the reasons in the logs. Knowing these reasons often aids in taking the required corrective action.
## Real-Time Container Metrics

**Command executed:** `docker stats`

| Metric         | Actual Observation                       |
| -------------- | ---------------------------------------- |
| Container Name | client-website                           |
| CPU Usage      | 0.00%                  |
| Memory Usage   | 2.727MiB|
| Memory Limit   | 1.859GiB                 |
| Network I/O    | 4.49kB / 5.95kB                |

### Analysis

Docker Stats displays the resource utilization of containers in real time. CPU and memory usage of a container give the engineer an idea about the resources being utilized by the container in the process of servicing requests.

## Evidence

* `screenshots/container-metrics.png`
