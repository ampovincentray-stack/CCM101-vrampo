# Cloud Infrastructure Components Analysis

## 1. Compute Resources
- **Purpose:** Compute resources provide the processing power required to run operating systems, application logic, algorithms, and workload instructions.
- **Importance in Cloud:** They act as the primary brain of cloud deployments, enabling scalable virtual instances (VMs or containers) that dynamically scale depending on user demand.
- **KillerCoda Context:** In KillerCoda, the virtualized CPU cores (e.g., AMD/Intel vCPUs) allocated to our terminal session represent virtual compute instances provided by a hypervisor.

## 2. Storage Resources
- **Purpose:** Storage resources persist data, files, application code, databases, and configuration settings across system restarts.
- **Importance in Cloud:** Centralized cloud storage guarantees high availability, data redundancy, backups, and shared access across multiple distributed compute nodes.
- **KillerCoda Context:** The block storage mounted at `/` (root directory) and inspected via `df -h` provides disk space where files, packages, and system logs are stored.

## 3. Networking Resources
- **Purpose:** Networking components interconnect servers, route traffic, manage bandwidth, isolate resources, and establish secure external access.
- **Importance in Cloud:** Networks allow compute and storage systems to communicate globally via Virtual Private Clouds (VPCs), subnets, firewalls, and load balancers.
- **KillerCoda Context:** The virtual network interfaces (`eth0`, `lo`) and IP address configurations viewed through `ip a` allow our web browser to send commands directly to the cloud container/VM.

## 4. Operating System
- **Purpose:** The OS acts as an intermediary layer managing software applications and abstracting hardware resources (CPU, RAM, Storage).
- **Importance in Cloud:** It provides the environment for executing cloud-native software, microservices, and management scripts smoothly.
- **KillerCoda Context:** Linux (Ubuntu) serves as the host platform in our KillerCoda session, providing CLI access via bash shell to interact directly with system configurations.
