# Day#11

## Install Windows on a VM
To install Windows on a virtual machine (VM) in ESXi, you will need to follow these steps:

+ Create a new VM in ESXi using the vSphere Client or the vSphere Web Client.
+ During the creation process, specify the operating system type as "Microsoft Windows" and select the version of Windows you want to install.
+ Allocate sufficient resources (e.g., CPU, memory, storage) to the VM to meet the minimum requirements for the version of Windows you are installing.
+ Attach the Windows installation media (e.g., an ISO file or a DVD) to the VM.
+ Power on the VM and boot from the installation media.
+ mFollow the prompts to install Windows on the VM.
Note that you will need a valid license key for the version of Windows you are installing. You can either purchase a new license key or use an existing one if you have one available.

## Install VMWare Tools

VMware Tools is a suite of utilities that enhances the performance of a virtual machine (VM) running on the VMware vSphere platform. It includes drivers and software that optimize the performance of the VM's operating system and applications, as well as tools for improving the VM's integration with the host system.

To install VMware Tools on a VM, you will need to follow these steps:

+ Power on the VM and log in to the operating system.
+ Connect the VMware Tools ISO file to the VM. This can usually be done by right-clicking on the VM in the vSphere Client or vSphere Web Client and selecting "Install VMware Tools".
+ Mount the VMware Tools ISO file as a virtual CD/DVD drive in the VM.
+ In the VM, open the mounted VMware Tools ISO file and run the installation program (e.g., "setup.exe" on Windows or "install.sh" on Linux).
+ Follow the prompts to install VMware Tools on the VM.
Note that you may need to restart the VM after installing VMware Tools in order for the changes to take effect. Additionally, some versions of VMware Tools may require you to update the VM's operating system and/or kernel in order to be compatible.

## Important Resources

Now let's start with [Day#12](Day%4012.md)