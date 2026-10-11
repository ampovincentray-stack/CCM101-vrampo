# Container Observability Report

## 1. Application Logs

**Command executed:** `docker logs client-website`

### HTTP 404 Error Log

Paste the exact line from your terminal that records the request to `/hidden-admin-page` and the HTTP 404 status.

### Why Application Logs Are Important

Application logs are important because they record requests, errors, and other events that help engineers identify what went wrong. By examining these logs, an engineer can investigate failed requests, determine possible causes, and choose appropriate troubleshooting steps.

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

The `docker stats` command provides real-time information about container resource consumption. The CPU percentage and memory usage help an engineer assess whether the container is consuming significant resources while serving web requests.

## Evidence

* `screenshots/container-metrics.png`
