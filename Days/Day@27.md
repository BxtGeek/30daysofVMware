
# Day#27

## ESXCLi and ESXi Shell Commands for VMware
ESXCLI and ESXi Shell are two different command-line interfaces (CLI) for managing VMware ESXi hosts. Both interfaces provide a wide range of commands for managing and troubleshooting your ESXi environment.

### ESXCLI commands:

+ esxcli is a powerful command-line interface for managing and troubleshooting ESXi hosts. It can be used to perform various management tasks, such as configuring, troubleshooting, and maintaining your ESXi host and virtual machines.
+ esxcli commands are structured as follows: esxcli <namespace> <cmd> <cmd options>
+ Examples of esxcli commands include:
++ esxcli network firewall ruleset list: lists all the firewall rulesets
++ esxcli storage core device list: lists all storage devices
++ esxcli software vib list: lists all the VIBs (VMware Installation Bundles) that are installed on the host

### ESXi Shell commands:

+ ESXi Shell is a command-line interface that provides access to a limited set of ESXi host commands. It can be used to perform basic management tasks, such as managing files and directories, configuring network settings, and monitoring system processes.
+ Examples of ESXi shell commands include:
++ cd /: changes the current directory to the root directory
++ ls: lists the files and directories in the current directory
++ vim-cmd vmsvc/getallvms: lists all the virtual machines running on the host
++ esxcfg-info: shows system information and configuration settings for the host

Overall, both esxcli and ESXi Shell commands can be useful for managing and troubleshooting your ESXi environment. However, esxcli is more powerful and versatile, providing a wide range of commands for advanced management tasks, while ESXi Shell is more suited for basic management tasks.
 
## VMWare vCenter Converter

## Important Resources

Now let's start with [Day#28](Day%4028.md)
