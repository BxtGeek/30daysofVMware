# Day#23

## Distributed Resource Scheduler (DRS)

Distributed Resource Scheduler (DRS) is a feature of VMware vSphere that enables automatic balancing of resources such as CPU and memory across the hosts in a VMware cluster. It works by constantly monitoring the resource usage of the virtual machines in the cluster and making adjustments as needed to ensure that resources are used efficiently.

DRS uses an algorithm to determine the best host to run a virtual machine based on the current resource usage of the hosts and the resource requirements of the virtual machine. This allows for optimal utilization of resources and helps to prevent resource contention.

DRS also provides advanced features such as:

+ Automated initial placement: When a new virtual machine is created, DRS suggests the best host and resource pool to run the VM
+ Automated load balancing: DRS automatically balances the load across the hosts in the cluster by migrating virtual machines between hosts
+ Power Management: DRS uses the power management capabilities of the hosts to save energy, it can use the data of the workload to ensure that the hosts are not over- or under-utilized
+ vMotion: DRS uses vMotion to migrate virtual machines between hosts without any interruption of service

DRS can be easily configured and managed through the vCenter Server, which provides a centralized management point. It works in conjunction with VMware High Availability (HA) to ensure the availability of virtual machines and the efficient use of resources.

## The sequence of Starting and Shutting VMWare vSphere Environment
The sequence of starting and shutting down a VMware vSphere environment depends on the specific components that are in use and the desired level of availability. However, a general sequence would be as follows:

+ Start vCenter Server: This is the central management component that is used to manage the VMware cluster. It should be started first to ensure that it is available to manage the other components.

+ Start ESXi hosts: These are the physical servers that run the VMware vSphere hypervisor and host the virtual machines. They should be started in a specific order, if there is any dependency between them.

+ Start virtual machines: Once the ESXi hosts are running, virtual machines can be started. They can be started manually or automatically through the vCenter Server.

+ Start any additional services or applications: If there are any additional services or applications that are running in the environment, they should be started after the virtual machines are running.

+ Shutting down: Shutting down the environment should be done in the reverse order, starting with stopping any additional services or applications, then stopping the virtual machines, ESXi hosts and finally shutting down vCenter Server.

## Datastore clusters

A Datastore Cluster in VMware vSphere is a collection of datastores that are managed together as a single entity. It allows administrators to create a pool of storage resources that can be used by virtual machines, and it provides advanced features such as:

+ Storage DRS (Storage Distributed Resource Scheduler): This feature automatically balances the load of the datastores in the cluster by migrating virtual machines between them based on the current usage and capacity of the datastores.

+ Storage vMotion: This feature allows administrators to move virtual machines and their virtual disks between datastores in the cluster without any interruption of service.

+ Storage I/O Control (SIOC): This feature allows administrators to set priorities for the virtual machines running on the datastores in the cluster, which ensures that the virtual machines with the most important workloads receive the highest I/O priority.

+ Profile-driven storage: This feature allows administrators to assign storage capabilities to virtual machines, such as performance and availability.

Datastore clusters are used to improve the availability, performance, and manageability of the storage resources in a vSphere environment. They are created and managed through the vCenter Server, which provides a centralized management point. This makes it easy to manage the storage resources and monitor the performance of the virtual machines running on the datastores.

## Important Resources

Now let's start with [Day#24](Day%4024.md)
