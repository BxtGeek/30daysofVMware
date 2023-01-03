# Day#9

## First VM on ESXi

To create your first virtual machine (VM) on an ESXi server, follow these steps:

+ Connect to the ESXi server: You can connect to the ESXi server using a web browser or a client software like VMware vSphere Client. To connect using a web browser, type the IP address or hostname of the ESXi server in the address bar and log in using the root username and password that you created during the installation.

+ Create a new virtual machine: To create a new VM, click on the "Create a New Virtual Machine" button in the vSphere Client or the web interface. This will open the New Virtual Machine Wizard.

+ Specify the virtual machine configuration: In the wizard, you will need to specify the configuration of the VM, including the operating system, the number of virtual CPUs and memory, and the virtual hardware. You can also specify the location for the VM files and the storage policies to be used.

+ Install the operating system: Once you have configured the VM, you will need to install the operating system. You can do this by booting the VM from an ISO image or a bootable USB drive. Follow the prompts to install the operating system on the VM.

+ Configure the VM: After the operating system is installed, you can configure the VM as needed. This may include installing applications, configuring networking, and setting up users and permissions.

+ Power on the VM: Once you have finished configuring the VM, you can power it on by clicking the "Power on" button in the vSphere Client or the web interface.

Note that the exact steps and options for creating and configuring a VM will vary depending on the version of the ESXi server you are using and the operating system and applications you are installing on the VM. It is recommended to refer to the VMware documentation for detailed instructions on creating and configuring VMs on the ESXi server.

## Install Linux OS

To install Linux on a virtual machine (VM) on an ESXi server, follow these steps:

+ Connect to the ESXi server: You can connect to the ESXi server using a web browser or a client software like VMware vSphere Client. To connect using a web browser, type the IP address or hostname of the ESXi server in the address bar and log in using the root username and password that you created during the installation.

+ Create a new virtual machine: To create a new VM, click on the "Create a New Virtual Machine" button in the vSphere Client or the web interface. This will open the New Virtual Machine Wizard.

+ Specify the virtual machine configuration: In the wizard, you will need to specify the configuration of the VM, including the operating system, the number of virtual CPUs and memory, and the virtual hardware. You can also specify the location for the VM files and the storage policies to be used.

+ Install the operating system: Once you have configured the VM, you will need to install the operating system. To install Linux on the VM, you will need to have an ISO image of the Linux distribution that you want to install. You can either upload the ISO image to the ESXi server or store it on a local network share.

+ Boot from the ISO image: To boot from the ISO image, you will need to attach the ISO image to the VM as a CD/DVD drive. In the vSphere Client or the web interface, select the ISO image as the boot device for the VM.

+ Follow the installation prompts: When the VM boots from the ISO image, you will be presented with the Linux installation prompts. Follow the prompts to install Linux on the VM. This will involve selecting the installation language, partitioning the disk, and setting up the user accounts and other configuration options.

Note that the exact steps and options for installing Linux on a VM will vary depending on the version of the ESXi server you are using and the Linux distribution you are installing. It is recommended to refer to the documentation for the Linux distribution and the ESXi server for detailed instructions on the installation process.

## Important Resources

Now let's start with [Day#10](Day%409.md)