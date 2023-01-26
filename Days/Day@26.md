# Day#26

## Fault Tolerance

Fault Tolerance (FT) in VMware is a feature that provides continuous availability of virtual machines (VMs) in the event of a host failure. It ensures that VMs are protected against the failure of a single physical host by creating a secondary, identical copy of the VM, called a "secondary VM," on another host in the cluster. If the primary VM fails, the secondary VM automatically takes over and continues to run, providing a seamless experience for the end-user.

VMware vSphere Fault Tolerance (FT) can be implemented by using following features:

+ vSphere FT: This feature provides fault tolerance for individual virtual machines by creating a secondary, identical copy of the primary virtual machine.
+ vSphere High Availability (HA): This feature provides automatic failover for virtual machines in the event of a host failure.
+ vSphere Distributed Resource Scheduler (DRS): This feature balances the load across hosts in a cluster to ensure that virtual machines have the resources they need to run.

### How to implement vSphere High Availability (HA)
vSphere High Availability (HA) is a feature in VMware that provides automatic failover for virtual machines in the event of a host failure. Here are the basic steps to implement vSphere HA:

+ Create a cluster: Create a cluster of hosts that will participate in HA. This is done in the vSphere Web Client by going to the Hosts and Clusters view and creating a new cluster.
+ Configure shared storage: Ensure that all hosts in the cluster have access to shared storage, such as a SAN or NAS. This is necessary for HA to function properly.
+ Enable HA: In the vSphere Web Client, navigate to the cluster and click on the Configure tab. Under Services, click on the Edit button next to High Availability. Follow the prompts to enable HA and configure the settings.
+ Add hosts to the cluster: Once HA is enabled, add the hosts to the cluster.
+ Configure VM Monitoring: In the vSphere Web Client, navigate to the cluster and click on the Configure tab. Under Services, click on the Edit button next to High Availability. In the VM Monitoring settings, you can configure how often HA checks the state of virtual machines and how long it waits before marking a virtual machine as failed.
+ Add virtual machines to the cluster: Once the cluster is configured and the hosts are added, you can add virtual machines to the cluster. When you add a virtual machine to the cluster, it is automatically protected by HA.
+ Test the HA functionality: Once the configuration is done, you can test the HA functionality by simulating a host failure. This can be done by shutting down a host in the cluster or disconnecting it from the network. The virtual machines running on that host should automatically fail over to another host in the cluster and continue running. It is important to test the HA functionality to ensure that it is working as expected and that the virtual machines are properly protected in case of an actual host failure.

It's important to note that vSphere HA is not a replacement for a backup solution, it's a feature that provides high availability of the virtual machines in case of a host failure. It's highly recommended to test the HA functionality regularly, monitor the cluster and fine-tune the settings according to the environment needs.

### How to implement vSphere Distributed Resource Scheduler (DRS)
vSphere Distributed Resource Scheduler (DRS) is a feature in VMware that automatically balances the workloads of virtual machines across multiple hosts in a cluster. Here are the basic steps to implement vSphere DRS:

+ Create a cluster: Create a cluster of hosts that will participate in DRS. This is done in the vSphere Web Client by going to the Hosts and Clusters view and creating a new cluster.
+ Configure shared storage: Ensure that all hosts in the cluster have access to shared storage, such as a SAN or NAS. This is necessary for DRS to function properly.
+ Enable DRS: In the vSphere Web Client, navigate to the cluster and click on the Configure tab. Under Services, click on the Edit button next to Distributed Resource Scheduler. Follow the prompts to enable DRS and configure the settings.
+ Add hosts to the cluster: Once DRS is enabled, add the hosts to the cluster.
+ Configure DRS Automation level: In the vSphere Web Client, navigate to the cluster and click on the Configure tab. Under Services, click on the Edit button next to Distributed Resource Scheduler. Select the automation level that you want to use: Fully Automated, Manual, or Partially Automated.
+ Add virtual machines to the cluster: Once the cluster is configured and the hosts are added, you can add virtual machines to the cluster. When you add a virtual machine to the cluster, it is automatically managed by DRS.
+ Monitor the cluster: Once the configuration is done, monitor the cluster to ensure that DRS is properly balancing the workloads of the virtual machines. You can view the DRS recommendations, the current resource usage of the cluster, and the history of DRS actions in the vSphere Web Client.

It's important to note that DRS is a feature that provides load balancing across the hosts in a cluster and it doesn't guarantee high availability of the virtual machines. It's highly recommended to fine-tune the DRS settings according to the environment needs.

## Important Resources
+ [How to Setup vCenter Server High Availability (HA)](https://www.youtube.com/watch?v=t1aYx8fBcQo)
+ [Understanding of vSphere High Availability(HA)](https://www.youtube.com/watch?v=daAkEw7XHO8)
+ [VMware High Availability Explained](https://www.youtube.com/watch?v=pQmKd0jGIiI)
+ [Understanding of vSphere Distributed Resource Scheduler(DRS)](https://www.youtube.com/watch?v=fn_GnnQtDEc)
+ [VMware DRS (Distributed Resource Scheduler)](https://www.youtube.com/watch?v=PUqvY-Fhhvc)

Now let's start with [Day#27](Day%4027.md)
