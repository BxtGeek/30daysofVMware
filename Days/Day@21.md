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

## Important Resources

Now let's start with [Day#22](Day%4022.md)
