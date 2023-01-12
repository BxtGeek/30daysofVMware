# Day#12

## Review VMs and Modify Resources

To review and modify the resources of a virtual machine (VM) in ESXi, you will need to follow these steps:

+ Connect to your ESXi host using the vSphere Client or the vSphere Web Client.
+ In the left-hand navigation panel, click on the VM you want to review and modify.
+ In the right-hand panel, click on the "Summary" tab.
+ Review the current resource allocation (e.g., CPU, memory, storage) of the VM.
+ To modify the resources, click on the "Edit" button next to the relevant resource (e.g., "CPUs", "Memory", "Hard disk").
+ In the "Edit Virtual Machine" dialog box, adjust the resource allocation as needed and click "OK".
Note that modifying the resources of a VM may require you to shut down the VM in order for the changes to take effect. Be sure to save any work and shut down the VM before modifying its resources. Additionally, be aware that changing the resources of a VM may have an impact on the performance of the VM and the overall workload of the host system.

## VM Snapshots

A VM snapshot is a saved state of a virtual machine (VM) at a specific point in time. VM snapshots can be useful in various scenarios, such as:

+ Creating a point-in-time backup of a VM
+ Testing changes to a VM without affecting its current state
+ Saving a VM's state before making changes, so that you can revert to the previous state if needed

To create a VM snapshot in ESXi, you can use the vSphere Client or the vSphere Web Client. Here is the basic process:

+ Connect to the vSphere Client or vSphere Web Client.
+ Select the VM for which you want to create a snapshot.
+ Click the "Snapshots" tab.
+ Click the "Take Snapshot" button.
+ Enter a name and optional description for the snapshot.
+ Choose whether to include memory and/or quiesced data in the snapshot.
+ Click "OK" to create the snapshot.
Note: Depending on the size of the VM and the amount of data that needs to be saved, creating a snapshot may take some time. During this time, the VM may be unavailable or may run slower than usual.

## Important Resources
+ [VMWare Snapshots Explained](https://www.youtube.com/watch?v=DQutP_-2j3g)
+ [File Snapshots](https://www.youtube.com/watch?v=gZlGaD-DtKo)
+ [Snapshots vs Backups vs Replications](https://www.youtube.com/watch?v=BcA13YbUv-4)


Now let's start with [Day#13](Day%4013.md)
