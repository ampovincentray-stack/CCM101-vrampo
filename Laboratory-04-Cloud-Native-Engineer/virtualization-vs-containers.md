# Virtual Machines vs Containers

| Category            | Virtual Machines                                                                                  | Containers                                                                                                    |
| ------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Architecture        | 	All virtual machines have their own guest OS appropriate for that VM.       | The kernel of the host OS is shared by containers but applications and its respective dependencies are isolated from each other. |
| Boot Time           | Normally, a VM takes a few minutes to boot itself up.                     | Usually containers are able to start in seconds, as they do not require booting a separate OS.         |
| Resource Efficiency | Efficiency	VM consumes more CPU, memory, and storage than would be needed because of the guest operating system used by the VM..          | In most cases, containers are lightweight since they make use of the host OS kernel.           |
| Isolation Level     | VM makes use of the virtualization technology and allows use of isolated environments. | By using the host operating system kernel, containers are providing the capability of process level isolation at the same time.                    |

## Summary

Web applications utilize containers due to their cost-effective attributes, being lighter and booting faster than conventional Virtual Machines. Unlike Virtual Machines, containers do not have to maintain multiple guest OS for their applications and use lesser resources. Through Docker, the process of deploying applications across similar systems has become that much easier and smoother.
