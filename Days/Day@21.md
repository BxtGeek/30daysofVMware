# Day#21

## Migrating VM without VMWare cluster (Cold)

Cold migration is the process of moving a virtual machine (VM) from one host to another without the use of VMware vSphere clusters or vMotion. This type of migration is also known as a "cold clone" or "cold transfer."

There are several ways to perform a cold migration of a VM without the use of a cluster:

+ Using VMware Converter: VMware Converter is a tool that can be used to create a copy of a VM and move it to another host. The process involves creating a virtual machine disk (VMDK) file of the source VM, and then importing that VMDK file into the destination host.

+ Using a backup and restore process: This method involves creating a backup of the source VM and restoring it to the destination host. This can be done using third-party backup software or using built-in features such as VMware Data Protection.

+ Using a file copy method: This method involves copying the VMDK files and configuration files of the source VM to the destination host. This can be done manually, or by using a script or automation tool.

It's important to note that during a cold migration, the VM will be powered off and will not be available during the migration process, this could lead to service disruption. Additionally, due to the time it takes to copy data over the network and to reconfigure the VM on the destination host, the cold migration process can take longer than other types of migration.

In order to minimize the downtime, it's recommended to plan the migration in a low usage period, also to test the migration process in a development environment before performing it in production.


## vMotion

vMotion is a feature in VMware vSphere that allows for the live migration of virtual machines (VMs) from one host to another without any interruption of service. This is accomplished by allowing the VM's memory and virtual disk files to be moved from one host to another while the VM is still running. vMotion is supported by vSphere clusters, which are groups of hosts that are managed together and share resources such as storage and network.

To set up vMotion in vCenter, the following steps should be followed:

+ Create a vSphere cluster: In vCenter, go to the "Hosts and Clusters" view and create a new cluster by right-clicking on a datacenter and selecting "New Cluster." Give the cluster a name and select the hosts that will be included in the cluster.

+ Enable vMotion on the vSphere cluster: Once the cluster is created, go to the "Configure" tab and select "vMotion." Enable vMotion by checking the box and configure the network settings as needed.

+ Configure shared storage: vMotion requires shared storage that is accessible to all hosts in the cluster. The shared storage should be configured and connected to the hosts in the cluster.

+ Migrate VMs: Once vMotion is set up, you can use the "Migrate" option in the vCenter interface to move a VM from one host to another within the cluster. The VM's memory and virtual disk files will be transferred over the network, allowing for a seamless migration.

+ Configure vMotion Network: vMotion requires a dedicated network for migration, it's recommended to use a separate vSwitch and assign a separate vlan for vMotion traffic.

It's important to note that vMotion requires compatible hardware and software, ensure that all hosts in the cluster are running compatible versions of vSphere and that the hosts have compatible processors. Additionally, ensure that the network infrastructure is configured to support vMotion traffic.

By using vMotion, administrators can improve the availability and manageability of their virtualized environments by allowing for the live migration of VMs between hosts without interruption of service. This can be useful for planned maintenance, load balancing and disaster recovery scenarios.

## Important Resources
+ [Introduction to the vMotion process](https://www.youtube.com/watch?v=0Q_MPVeuWgc)
+ [Migrate VMs from Vmware ESXi 5.5 to Vmware ESXi 6.7](https://www.youtube.com/watch?v=xQC0j5I7cX4)

Now let's start with [Day#22](Day%4022.md)
