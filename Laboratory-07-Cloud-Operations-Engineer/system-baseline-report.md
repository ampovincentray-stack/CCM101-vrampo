# System Baseline Report

## 1. Objective

The objective of this checkpoint is to establish a baseline of the Linux host's memory, disk capacity, CPU load, and running processes before deploying the Nginx container.

## 2. Memory Check

**Command executed:** `free -h`

* Total RAM: 7.7Gi
* Used RAM: 1.2Gi
* Available RAM: 4.8Gi

## 3. Disk Check

**Command executed:** `df -h /`

* Root filesystem capacity: 19G
* Used storage: 5.5g
* Available storage: 13G
* Disk usage: 30%

## 4. CPU and Process Check

**Command executed:** `top`

The `top` command displayed the active processes, CPU utilization, and system load. I observed the changing resource values to understand the server's condition.

## 5. Why Disk Space Matters

Checking disk space before a massive traffic surge is important because a full filesystem can prevent applications from writing logs, temporary files, and other required data, potentially causing service failures.

## 6. Evidence

* `screenshots/memory-check.png`
* `screenshots/disk-check.png`

