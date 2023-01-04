# Day#10

## VM Management

There are several ways to manage virtual machines (VMs) in ESXi, the hypervisor platform from VMware. Here are some of the main ways to manage VMs in ESXi:

+ vSphere Client: This is a graphical user interface (GUI) tool provided by VMware that allows you to connect to and manage your ESXi host and VMs. You can use the vSphere Client to create, delete, and modify VMs, as well as to perform other tasks such as configuring networking, storage, and security settings.

+ vSphere Web Client: This is a web-based version of the vSphere Client that allows you to manage your ESXi host and VMs from any device with a web browser.

+ vSphere APIs: VMware provides a set of APIs that allow you to automate VM management tasks using your own custom scripts or applications. You can use these APIs to perform tasks such as creating and deleting VMs, modifying their configuration, and migrating them between hosts.

+ PowerCLI: This is a command-line interface (CLI) tool provided by VMware that allows you to automate VM management tasks using PowerShell scripts. You can use PowerCLI to perform tasks such as creating and deleting VMs, modifying their configuration, and retrieving information about your ESXi host and VMs.

+ vCenter Server: This is a centralized management platform provided by VMware that allows you to manage multiple ESXi hosts and VMs from a single interface. You can use vCenter Server to perform tasks such as creating and deleting VMs, modifying their configuration, and migrating them between hosts.

## Update ESXi hostname

To update the hostname of an ESXi host, you will need to follow these steps:

+ Connect to your ESXi host using the vSphere Client or the vSphere Web Client.
+ In the left-hand navigation panel, click on the host.
+ In the right-hand panel, click on the "Configuration" tab.
+ In the "Software" section, click on the "General" tab.
+ Click on the "Edit" button next to the "Host name" field.
+ Enter the new hostname in the "Host name" field and click "OK".
+ Click on the "OK" button in the "Edit Host" dialog box to apply the changes.
Note that changing the hostname of an ESXi host will require a reboot of the host in order for the change to take effect. Be sure to save any work and shut down any running VMs before rebooting the host.

## Important Resources

Now let's start with [Day#11](Day%4011.md)