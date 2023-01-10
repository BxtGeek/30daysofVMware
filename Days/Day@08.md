# Day#8

## Download and Install ESXi Server (Hypervisor)

To download and install the ESXi server (also known as the hypervisor), follow these steps:

+ Download the ESXi installer: Go to the VMware website and download the latest version of the ESXi installer. You will need to create a VMware account if you don't already have one.

+ Create a bootable USB or DVD: Once the download is complete, use a tool like Rufus to create a bootable USB or DVD from the installer file.

+ Boot from the USB or DVD: Insert the bootable USB or DVD into the server and restart it. Make sure that the server is set to boot from the USB or DVD in the BIOS or UEFI settings.

+ Follow the installation prompts: The installation process will guide you through the steps to install the ESXi server. This will include setting up the server's network configuration, creating a root password, and selecting the storage devices to use for the ESXi installation.

+ Configure the ESXi server: After the installation is complete, you will need to configure the ESXi server to suit your needs. This will include creating virtual machines, setting up storage, and configuring networking.

Note that the exact steps may vary depending on the specific version of ESXi you are using and the hardware configuration of your server. It is recommended to refer to the VMware documentation for detailed instructions on the installation and configuration process.

## Configure ESXi Server

Once you have installed the ESXi server, you will need to configure it to suit your needs. Here are the general steps to configure the ESXi server:

+ Connect to the ESXi server: You can connect to the ESXi server using a web browser or a client software like VMware vSphere Client. To connect using a web browser, type the IP address or hostname of the ESXi server in the address bar and log in using the root username and password that you created during the installation.

+ Configure networking: The first step in configuring the ESXi server is to set up the networking. This includes creating virtual switches, assigning network adapters, and configuring VLANs (virtual LANs) as needed.

+ Create virtual machines: Next, you can create virtual machines on the ESXi server. This involves specifying the operating system and hardware resources for each virtual machine, as well as installing the operating system and any necessary applications.

+ Set up storage: You will also need to set up storage for the ESXi server. This includes creating datastores, assigning storage devices, and configuring storage policies as needed.

+ Manage users and permissions: You can create and manage users and groups on the ESXi server, as well as assign permissions to control access to the server and its resources.

+ Monitor and maintain the ESXi server: Finally, you will need to monitor and maintain the ESXi server to ensure that it is running optimally. This includes keeping the ESXi software and virtual machine hardware up-to-date, as well as monitoring performance and capacity usage.

Note that the exact steps and options for configuring the ESXi server will vary depending on your specific needs and the version of the ESXi server you are using. It is recommended to refer to the VMware documentation for detailed instructions on configuring the ESXi server.

## Important Resources
+ [How to Install VMware vSphere Hypervisor 8.0](https://www.youtube.com/watch?v=FlOJh8hesqA)
+ [How to Install VMware vSphere Hypervisor 7.0](https://www.youtube.com/watch?v=YhXsX4kJS3M)
+ [Before I do anything with VMware ESXi I do this first](https://www.youtube.com/watch?v=-1BMiYZfz38)
+ [vSphere 7 - How To Install and Configure VMware ESXi 7](https://www.youtube.com/watch?v=O0Xt_YrLrBA)

Now let's start with [Day#9](https://github.com/BxtGeek/30daysofVMware/blob/main/Days/Day%4009.md)
