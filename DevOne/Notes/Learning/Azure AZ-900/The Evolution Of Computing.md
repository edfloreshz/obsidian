# Dedicated

- Overpay for an underutilized server.
- Limited by your OS.
- Multiple apps can result in conflicts in resource sharing.
- You have a guarantee of security, privacy and full utility of underlying resources.

# VMs

- Hypervisor lets you run VMs within a physical server.
- Is shared by multiple customers.
- You pay a fraction of the server.
- You’ll overpay for an underutilized VM.
- Limited by the OS.

# Containers

- VM running in multiple containers.
- Docker Daemon is the software layer that lets your run multiple containers.
- Is more cost-effective.
- They share the same underlying OS but you can have different OSs for multiple containers.

# Functions

- A managed VMs running containers.
- This is known as **server-less compute**.
- You upload a piece of code and choose the amount of memory and duration.
- Only responsible for code and data.
- Very cost-effective, only pay for the time code is running, VMs only run when code needs to be executed.
- Cold Starts is a side-effect of this setup.