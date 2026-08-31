# Laboratory 02: Build the Cloud Infrastructure Blueprint

## Mission Overview
This laboratory activity focuses on exploring, assessing, and documenting core cloud infrastructure primitives (Compute, Storage, Networking, and IAM) using interactive cloud terminals and public cloud providers' documentation.

## Objectives
- Investigate Linux system specifications in a cloud-hosted environment.
- Categorize compute, storage, network, and identity services.
- Compare service offerings between AWS, Azure, and GCP.
- Design a high-level cloud architecture diagram.
- Build clean technical Markdown documentation inside GitHub.

## Cloud Infrastructure Components
- **Compute:** Execution environment for running virtual workloads.
- **Storage:** Data persistence layers for files and block-level access.
- **Networking:** Virtualized routing, IP assignment, and secure network traffic flow.
- **Identity:** Access control structures that manage authorization and authentication.

## Tools Used
- KillerCoda Interactive Linux Playground
- GitHub & Markdown
- Excalidraw (Diagramming)
- Linux CLI Diagnostics

## Linux Commands Executed
- `uname -r`: Display kernel details.
- `cat /etc/os-release`: Display operating system distribution info.
- `lscpu`: Retrieve CPU architecture and CPU core counts.
- `free -h`: Check system RAM utilization.
- `df -h`: Inspect mounted file system disk usage.
- `ip a`: Check network interface and IP configuration.

## Architecture Blueprint
![Cloud Architecture](screenshots/cloud-architecture.png)

## Skills Learned
- Navigating and auditing cloud-based Linux host environments via CLI.
- Mapping proprietary cloud vendor services to general computing primitives.
- Translating system components into visual architecture diagrams.

## Challenges Encountered
- Mapping vendor-specific cloud product naming variations.
- Configuring correct relative path references for repository markdown image rendering.
