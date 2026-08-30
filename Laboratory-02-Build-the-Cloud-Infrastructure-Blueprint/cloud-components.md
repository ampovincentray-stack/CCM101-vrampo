# Cloud Infrastructure Components

## Introduction

Cloud infrastructure is made up of different resources that work together to provide computing services. In the KillerCoda Linux environment, I was able to observe compute, storage, networking, and operating system resources. These components are important because they allow applications and services to run properly in a cloud environment.

---

## 1. Compute Resources

### Purpose

Compute resources provide the processing power needed to run applications, execute commands, and perform different tasks. The main compute resources observed in the Linux environment are the CPU and RAM.

### Importance in Cloud Computing

Compute resources are important in cloud computing because applications need processing power and memory to operate. Cloud providers allow organizations to increase or decrease compute resources depending on their workload. This makes cloud computing flexible and helps organizations use resources according to their needs.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment provides a virtual server with CPU and RAM resources. I used the `lscpu` command to examine the CPU information and the `nproc` command to determine the number of CPU cores. I also used the `free -h` command to check the available memory. These resources allow the Linux server to execute commands and run the activities required in this laboratory.

---

## 2. Storage Resources

### Purpose

Storage resources provide space for storing the operating system, applications, configuration files, and other data. In a Linux environment, storage is commonly provided through disk or filesystem resources.

### Importance in Cloud Computing

Storage is important in cloud computing because applications and users need a reliable place to save data. Cloud storage allows organizations to store files and information without maintaining physical storage devices themselves. It can also provide scalability, allowing storage capacity to increase as data requirements grow.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux server has disk storage that is used by the operating system and the files needed to run the laboratory environment. I used the `df -h` command to check the disk capacity, available space, used space, and mounted filesystems. This showed how storage is organized and used by the Linux server.

---

## 3. Networking Resources

### Purpose

Networking resources allow computers, servers, applications, and users to communicate with one another. Important networking information in the Linux environment includes the hostname and IP address.

### Importance in Cloud Computing

Networking is important in cloud computing because cloud resources need to communicate with users and other services. A properly configured network allows users to access applications and allows different cloud components to exchange information. Networking also helps connect cloud servers to the internet and other systems.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment has networking resources that allow the server to communicate within its environment. I used the `hostname` command to identify the server and the `hostname -I` command to determine its IP address. These commands helped me understand how the Linux server is identified and connected through a network.

---

## 4. Operating System

### Purpose

The operating system manages the computer's hardware and software resources. It provides the environment where users can execute commands and applications can run.

### Importance in Cloud Computing

The operating system is important in cloud computing because cloud servers need an operating system to manage compute, storage, networking, and applications. Linux is widely used in server environments because it provides command-line tools and system administration features that are useful for managing cloud infrastructure.

### Relation to the KillerCoda Linux Environment

The KillerCoda Playground provides a Linux-based server environment. I used the `cat /etc/os-release` command to identify the operating system and the `uname -r` command to identify its kernel version. The Linux operating system allows me to interact with the cloud server through the terminal and perform the commands required for this laboratory activity.

---

## Summary

The four infrastructure components work together to create a functional cloud environment. Compute resources provide processing power, storage resources provide space for data, networking resources allow communication, and the operating system manages the underlying resources. The KillerCoda Linux environment provided a practical example of these components and helped me understand how they work together in a cloud computing environment.
