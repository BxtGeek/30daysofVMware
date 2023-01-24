# Day#25

## VM Export and Import (OVF)
VM Export and Import (OVF) is a feature in VMware vSphere that allows users to export a virtual machine (VM) to a file in the OVF format, and then import that file to create a new VM. OVF is an open standard format for packaging and distributing virtual appliances, it is designed to make it easy to move virtual machines between different virtualization platforms.

## How to Export VM(OVF)
Here are the steps to export a VM as an OVF file in VMware vSphere:

+ Open the vSphere Client and log in to your vCenter Server/
+ Navigate to the inventory and select the virtual machine that you want to export.
+ Right-click on the virtual machine and select "All vCenter Actions" and then "Export OVF Template."
+ In the "Export OVF Template" wizard, you can specify the location where you want to save the OVF file and select the components you want to include in the export.
+ Click on "Next" and review the settings, then click "Finish" to start the export process.
+ Once the export process completes, you will find the OVF file in the specified location.
+ You can now use the OVF file to import the virtual machine to another vSphere environment or another virtualization platform that supports the OVF format.

## How to Import VM(OVF)
Here are the steps to import a VM as an OVF file in VMware vSphere:

+ Open the vSphere Client and log in to your vCenter Server.
+ Select "File" in the vSphere client and then select "Deploy OVF Template."
+ In the "Deploy OVF Template" wizard, browse and select the OVF file that you want to import.
+ Review the details of the OVF template, and select the options for the virtual hardware, storage, and network settings of the virtual machine.
+ Click on "Next" and review the settings, then click "Finish" to start the import process.
+ Once the import process completes, you will find the virtual machine in the inventory.
+ You can now power on the virtual machine, customize it as needed, and start using it.

## Important Resources
+ [How to Export\Import VM in OVF format in VMware Workstation](https://www.youtube.com/watch?v=WY11A-eyJWY)
+ [What is Ova in VMware? || How to upload OVA in VMware?](https://www.youtube.com/watch?v=W9B_Iy6iGsM)
+ [How to Export\Import VM in OVF format Using VMware OVF Tool](https://www.youtube.com/watch?v=uNbHy394-SA)

Now let's start with [Day#26](Day%4026.md)
