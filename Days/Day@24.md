# Day#24

## VM Cloning
VMware VM Cloning is a feature that allows users to create an exact copy of an existing virtual machine (VM) in VMware vSphere. The clone is an independent and fully functional VM that can be used for a variety of purposes, such as creating a test environment, deploying multiple VMs with similar configurations, or creating backups. The process of cloning a VM involves creating a copy of the virtual machine's configuration file and all of its associated files, such as virtual disks. The clone can then be customized as needed and powered on to create a new, independent VM.

## How to clone VM in vCenter
Here are the steps to clone a VM in vCenter:

+ Open the vSphere Client and log in to your vCenter Server.
+ Navigate to the inventory and select the virtual machine that you want to clone.
+ Right-click on the virtual machine and select "Clone."
+ In the "Clone Virtual Machine" wizard, select "Full Clone" if you want to create an independent copy of the virtual machine, or "Linked Clone" if you want to create a copy that shares virtual disks with the original virtual machine.
+ Select the destination for the cloned virtual machine. You can either choose to create the clone in the same folder as the original virtual machine, or you can choose a different folder or datacenter.
+ Enter a name for the cloned virtual machine, and select the host or cluster on which the clone will run.
+ Select the datastore where the virtual disk files of the cloned virtual machine will be stored.
+ Customize the clone as needed, such as changing the network settings, and click Next.
+ Review the settings and click Finish to start the cloning process.

Once the cloning process completes, you can power on the cloned virtual machine and start using it as a separate and independent virtual machine.

## VM Templates
VMware VM Templates are pre-configured virtual machines that can be used as a starting point for creating new virtual machines. A VM template contains a fully installed and configured operating system and any additional software that is needed for the virtual machine to function. When a new virtual machine is created from a template, the virtual machine is an exact copy of the template, including the operating system, applications, and configurations. This allows users to quickly deploy multiple virtual machines with the same configuration, without the need to manually install and configure the operating system and software on each virtual machine.

## How to create VM Templates
Here are the steps to create a VM template in vCenter:

+ Open the vSphere Client and log in to your vCenter Server.
+ Navigate to the inventory and select the virtual machine that you want to use as the basis for the template.
+ Right-click on the virtual machine and select "All vCenter Actions" and then "Convert to Template."
+ In the "Convert Virtual Machine to Template" wizard, review the settings and click Finish to start the conversion process.
+ Once the conversion process completes, the virtual machine will be removed from the inventory and replaced with a template.
+ You can find the newly created template under the "Template" folder in the inventory, you can use the template to create new virtual machines.
+ You can also customize the template before creating new VMs from it, like changing the name, adding new hardware, changing the network settings.

## Difference between VM Clone and VM Templates
The main difference between a VM Clone and a VM Template is the purpose and the resulting object.

A VM Clone is a copy of an existing virtual machine (VM) in VMware vSphere. The clone is an independent and fully functional VM that can be used for a variety of purposes, such as creating a test environment, deploying multiple VMs with similar configurations, or creating backups. The clone can be customized as needed and powered on to create a new, independent VM.

On the other hand, VM Templates are pre-configured virtual machines that can be used as a starting point for creating new virtual machines. A VM template contains a fully installed and configured operating system and any additional software that is needed for the virtual machine to function. When a new virtual machine is created from a template, the virtual machine is an exact copy of the template, including the operating system, applications, and configurations. This allows users to quickly deploy multiple virtual machines with the same configuration, without the need to manually install and configure the operating system and software on each virtual machine.
![Uploading screely-1674559365078.png…]()
In summary, a VM Clone is a standalone virtual machine that is an exact copy of an existing virtual machine with the ability to be customized and powered on independently. A VM Template is a preconfigured virtual machine that serves as a blueprint for creating new virtual machines, it does not have the ability to be powered on and is used for fast deployment of similar virtual machines.

