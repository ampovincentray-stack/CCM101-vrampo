# System Baseline Report

## 1. Objective

The main objective of this checkpoint is to come up with a baseline for memory usage, disk usage, CPU usage, and processes running on a Linux host prior to deployment of the Nginx container.

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

The "top" command shows all the processes that are active, CPU usage, and the system load. I noted all the changing parameters to understand how the server was working.
## 5. Why Disk Space Matters

Checking how much space is available on the disk before a sudden spike in traffic is important because an unresponsive filesystem might keep the applications from logging information, and thus failures may occur.

## 6. Evidence

* `screenshots/memory-check.png`
* `screenshots/disk-check.png`

