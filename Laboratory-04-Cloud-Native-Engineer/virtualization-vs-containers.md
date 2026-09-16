# Virtual Machines vs Containers

| Category            | Virtual Machines                                                                                  | Containers                                                                                                    |
| ------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Architecture        | Each VM includes a guest operating system that runs on a virtualized hardware environment.        | The kernel of the host OS is shared by containers but applications and its respective dependencies are isolated from each other. |
| Boot Time           | VMs usually take minutes to start because an operating system needs to boot.                      | Usually containers are able to start in seconds, as they do not require booting a separate OS.         |
| Resource Efficiency | VMs generally require more CPU, memory, and storage because each VM includes a guest OS.          | In most cases, containers are lightweight since they make use of the host OS kernel.           |
| Isolation Level     | VMs provide hardware-level virtualization and stronger separation between operating environments. | By using the host operating system kernel, containers are providing the capability of process level isolation at the same time.                    |

## Summary

Web applications utilize containers due to their cost-effective attributes, being lighter and booting faster than conventional Virtual Machines. Unlike Virtual Machines, containers do not have to maintain multiple guest OS for their applications and use lesser resources. Through Docker, the process of deploying applications across similar systems has become that much easier and smoother.
