# Azure Fundamentals Part 1
## What is Cloud Computing?
It's the delivery of computing services over the internet, which is otherwise known as the cloud. These services include servers, storage, databases, networking, software, analytics, and intelligence. 
#### Benefits of cloud computing
**Reliability**: Depending on the service-level agreement that you choose, your cloud-based applications can provide a continuous user experience with no apparent downtime even when things go wrong.

**Scalability**: Applications in the cloud can be scaled in two ways, while taking advantage of autoscaling:

**Vertically**: Computing capacity can be increased by adding RAM or CPUs to a virtual machine.
Horizontally: Computing capacity can be increased by adding instances of a resource, such as adding more virtual machines to your configuration.
Elasticity: Cloud-based applications can be configured to always have the resources they need.

**Agility**: Cloud-based resources can be deployed and configured quickly as your application requirements change.

**Geo-distribution**: Applications and data can be deployed to regional datacenters around the globe, so your customers always have the best performance in their region.

**Disaster recovery**: By taking advantage of cloud-based backup services, data replication, and geo-distribution, you can deploy your applications with the confidence that comes from knowing that your data is safe in the event that disaster should occur.

#### Cloud Computing Model
|Computing model	| Description |
|---------------- |-------------|
|IaaS |This cloud service model is the closest to managing physical servers. A cloud provider keeps the hardware up to date, but operating system maintenance and network configuration is left to the cloud tenant. For example, Azure virtual machines are fully operational virtual compute devices running in Microsoft's datacenters. An advantage of this cloud service model is rapid deployment of new compute devices. Setting up a new virtual machine is considerably faster than procuring, installing, and configuring a physical server.|
|PaaS	|This cloud service model is a managed hosting environment. The cloud provider manages the virtual machines and networking resources, and the cloud tenant deploys their applications into the managed hosting environment. For example, Azure App Services provides a managed hosting environment where developers can upload their web applications without having to deal with the physical hardware and software requirements.|
|SaaS	|In this cloud service model, the cloud provider manages all aspects of the application environment, such as virtual machines, networking resources, data storage, and applications. The cloud tenant only needs to provide their data to the application managed by the cloud provider. For example, Office 365 provides a fully working version of Office that runs in the cloud. All that you need to do is create your content, and Office 365 takes care of everything else.|
