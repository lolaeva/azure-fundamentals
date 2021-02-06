# Azure Fundamentals Part 1: Describe core Azure concepts
# What is Cloud Computing?
It's the delivery of computing services over the internet, which is otherwise known as the cloud. These services include servers, storage, databases, networking, software, analytics, and intelligence. 

## Benefits of cloud computing
**Reliability**: Depending on the service-level agreement that you choose, your cloud-based applications can provide a continuous user experience with no apparent downtime even when things go wrong.

**Scalability**: Applications in the cloud can be scaled in two ways, while taking advantage of autoscaling:

**Vertically**: Computing capacity can be increased by adding RAM or CPUs to a virtual machine.
Horizontally: Computing capacity can be increased by adding instances of a resource, such as adding more virtual machines to your configuration.
Elasticity: Cloud-based applications can be configured to always have the resources they need.

**Agility**: Cloud-based resources can be deployed and configured quickly as your application requirements change.

**Geo-distribution**: Applications and data can be deployed to regional datacenters around the globe, so your customers always have the best performance in their region.

**Disaster recovery**: By taking advantage of cloud-based backup services, data replication, and geo-distribution, you can deploy your applications with the confidence that comes from knowing that your data is safe in the event that disaster should occur.

## Cloud Computing Model
Infrastructure as a service (IaaS), platform as a service (PaaS), and software as a service (SaaS) are the different cloud service models. 
|Computing model	| Description |
|---------------- |-------------|
|IaaS |This cloud service model is the closest to managing physical servers. A cloud provider keeps the hardware up to date, but operating system maintenance and network configuration is left to the cloud tenant. For example, Azure virtual machines are fully operational virtual compute devices running in Microsoft's datacenters. An advantage of this cloud service model is rapid deployment of new compute devices. Setting up a new virtual machine is considerably faster than procuring, installing, and configuring a physical server.|
|PaaS	|This cloud service model is a managed hosting environment. The cloud provider manages the virtual machines and networking resources, and the cloud tenant deploys their applications into the managed hosting environment. For example, Azure App Services provides a managed hosting environment where developers can upload their web applications without having to deal with the physical hardware and software requirements.|
|SaaS	|In this cloud service model, the cloud provider manages all aspects of the application environment, such as virtual machines, networking resources, data storage, and applications. The cloud tenant only needs to provide their data to the application managed by the cloud provider. For example, Office 365 provides a fully working version of Office that runs in the cloud. All that you need to do is create your content, and Office 365 takes care of everything else.|

![iaas-paas-saas-expanded](https://user-images.githubusercontent.com/46975718/106366110-c0e69a00-634a-11eb-8c09-ee93af2953db.png)

### Shared Responsibility
![shared-responsibility](https://user-images.githubusercontent.com/46975718/106366111-c0e69a00-634a-11eb-871c-a743d6f3f33a.png)

## What is serverless computing?
Overlapping with PaaS, serverless computing enables developers to build applications faster by eliminating the need for them to manage infrastructure. With serverless applications, the cloud service provider automatically provisions, scales, and manages the infrastructure required to run the code. Serverless architectures are highly scalable and event-driven. They use resources only when a specific function or trigger occurs.

In understanding the definition of serverless computing, it's important to note that servers are still running the code. The serverless name comes from the fact that the tasks associated with infrastructure provisioning and management are invisible to the developer. This approach enables developers to increase their focus on the business logic and deliver more value to the core of the business. Serverless computing helps teams increase their productivity and bring products to market faster. It allows organizations to better optimize resources and stay focused on innovation.

## What are public, private, and hybrid clouds?
There are three deployment models for cloud computing: public cloud, private cloud, and hybrid cloud. Each deployment model has different aspects that you should consider as you migrate to the cloud.

Deployment model |	Description
---------------- | -------------
Public cloud |	Services are offered over the public internet and available to anyone who wants to purchase them. Cloud resources like servers and storage are owned and operated by a third-party cloud service provider and delivered over the internet.
Private cloud	| Computing resources are used exclusively by users from one business or organization. A private cloud can be physically located at your organization's on-site datacenter. It also can be hosted by a third-party service provider.
Hybrid cloud	| This computing environment combines a public cloud and a private cloud by allowing data and applications to be shared between them.

The following image illustrates several of the cloud computing concepts that are presented in this unit. In this example, several factors are demonstrated when you're considering where to deploy a database server in a hybrid cloud environment. As your resources move from on-premises to off-premises, your costs are reduced, and your administration requirements decrease.

![cloud-computing-continuum](https://user-images.githubusercontent.com/46975718/106366109-bfb56d00-634a-11eb-9102-47e6db0db1cd.png)

# What is Azure?
Azure is a continually expanding set of cloud services that help your organization meet your current and future business challenges. Azure gives you the freedom to build, manage, and deploy applications on a massive global network using your favorite tools and frameworks.

* Offers:
  * Be ready for the future: Continuous innovation from Microsoft supports your development today and your product visions for tomorrow.
  * Build on your terms
  * Operate hybrid seamlessly
  * Trust your cloud
  
## Azure Services

![azure-services](https://user-images.githubusercontent.com/46975718/106366112-c17f3080-634a-11eb-9e2f-2e584cb54885.png)

* Compute
* Networking
* Storage
* Mobile
* Databases
* Web
* IoT
* Big data
* AI
* DevOps


# Azure architectural components
Organizing structure for resources in Azure has four levels: management groups, subscriptions, resource groups, and resources. The following image shows the top-down hierarchy of organization for these levels.

![hierarchy](https://user-images.githubusercontent.com/46975718/107111315-41802b80-6860-11eb-8f6a-adf2b484c700.png)

* Resources: Resources are instances of services that you create, like virtual machines, storage, or SQL databases.
* Resource groups: Resources are combined into resource groups, which act as a logical container into which Azure resources like web apps, databases, and storage accounts are deployed and managed.
* Subscriptions: A subscription groups together user accounts and the resources that have been created by those user accounts. For each subscription, there are limits or quotas on the amount of resources that you can create and use. Organizations can use subscriptions to manage costs and the resources that are created by users, teams, or projects.
* Management groups: These groups help you manage access, policy, and compliance for multiple subscriptions. All subscriptions in a management group automatically inherit the conditions applied to the management group.

## Azure subscriptions
Using Azure requires an Azure subscription. A subscription provides you with authenticated and authorized access to Azure products and services. It also allows you to provision resources. An Azure subscription is a logical unit of Azure services that links to an Azure account, which is an identity in Azure Active Directory (Azure AD) or in a directory that Azure AD trusts.

An account can have one subscription or multiple subscriptions that have different billing models and to which you apply different access-management policies. You can use Azure subscriptions to define boundaries around Azure products, services, and resources. There are two types of subscription boundaries:

* Billing boundary: This subscription type determines how an Azure account is billed for using Azure. You can create multiple subscriptions for different types of billing requirements. Azure generates separate billing reports and invoices for each subscription so that you can organize and manage costs.
* Access control boundary: Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. An example is that within a business, you have different departments to which you apply distinct Azure subscription policies. This billing model allows you to manage and control access to the resources that users provision with specific subscriptions.

### Create additional Azure subscriptions
You might want to create additional subscriptions for resource or billing management purposes. For example, you might choose to create additional subscriptions to separate:

* Environments: When managing your resources, you can choose to create subscriptions to set up separate environments for development and testing, security, or to isolate data for compliance reasons. This design is particularly useful because resource access control occurs at the subscription level.
* Organizational structures: You can create subscriptions to reflect different organizational structures. For example, you could limit a team to lower-cost resources, while allowing the IT department a full range. This design allows you to manage and control access to the resources that users provision within each subscription.
* Billing: You might want to also create additional subscriptions for billing purposes. Because costs are first aggregated at the subscription level, you might want to create subscriptions to manage and track costs based on your needs. For instance, you might want to create one subscription for your production workloads and another subscription for your development and testing workloads.
* Subscription limits (also): Subscriptions are bound to some hard limitations. For example, the maximum number of Azure ExpressRoute circuits per subscription is 10. Those limits should be considered as you create subscriptions on your account. If there's a need to go over those limits in particular scenarios, you might need additional subscriptions.

### Customize billing to meet your needs
If you have multiple subscriptions, you can organize them into invoice sections. Each invoice section is a line item on the invoice that shows the charges incurred that month. For example, you might need a single invoice for your organization but want to organize charges by department, team, or project.
![billing-structure-overview-expanded](https://user-images.githubusercontent.com/46975718/107111721-41cdf600-6863-11eb-9bc6-1943e780e88b.png)

## Azure management groups
If your organization has many subscriptions, you might need a way to efficiently manage access, policies, and compliance for those subscriptions. Azure management groups provide a level of scope above subscriptions. You organize subscriptions into containers called management groups and apply your governance conditions to the management groups. All subscriptions within a management group automatically inherit the conditions applied to the management group. Management groups give you enterprise-grade management at a large scale no matter what type of subscriptions you might have. All subscriptions within a single management group must trust the same Azure AD tenant.

### Hierarchy of management groups and subscriptions
You can build a flexible structure of management groups and subscriptions to organize your resources into a hierarchy for unified policy and access management.
![management-groups-and-subscriptions-expanded](https://user-images.githubusercontent.com/46975718/107111857-61195300-6864-11eb-8630-eb78a0ef4c2e.png)

### Important facts about management groups
* 10,000 management groups can be supported in a single directory.
* A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level.
* Each management group and subscription can support only one parent.
* Each management group can have many children.
* All subscriptions and management groups are within a single hierarchy in each directory.

## Azure resource groups
Resource groups are a fundamental element of the Azure platform. A resource group is a logical container for resources deployed on Azure. These resources are anything you create in an Azure subscription like VMs, Azure Application Gateway instances, and Azure Cosmos DB instances. All resources must be in a resource group, and a resource can only be a member of a single resource group. Many resources can be moved between resource groups with some services having specific limitations or requirements to move. Resource groups can't be nested. Before any resource can be provisioned, you need a resource group for it to be placed in.
### Logical grouping
Resource groups exist to help manage and organize your Azure resources. By placing resources of similar usage, type, or location in a resource group, you can provide order and organization to resources you create in Azure. Logical grouping is the aspect that you're most interested in here, because there's a lot of disorder among our resources.

#### Life cycle
If you delete a resource group, all resources contained within it are also deleted. Organizing resources by life cycle can be useful in nonproduction environments, where you might try an experiment and then dispose of it. Resource groups make it easy to remove a set of resources all at once.
#### Authorization
Resource groups are also a scope for applying **role-based access control (RBAC) permissions**. By applying RBAC permissions to a resource group, you can ease administration and limit access to allow only what's needed.

## Azure Resource Manager
Azure Resource Manager is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. You use management features like access control, locks, and tags to secure and organize your resources after deployment.
![consistent-management-layer-expanded](https://user-images.githubusercontent.com/46975718/107112044-b86bf300-6865-11eb-94af-86d5477d7814.png)
All capabilities that are available in the Azure portal are also available through PowerShell, the Azure CLI, REST APIs, and client SDKs. 

### The benefits of using Resource Manager
* Manage your infrastructure through declarative templates rather than scripts. A Resource Manager template is a JSON file that defines what you want to deploy to Azure.
* Deploy, manage, and monitor all the resources for your solution as a group, rather than handling these resources individually.
* Redeploy your solution throughout the development life cycle and have confidence your resources are deployed in a consistent state.
* Define the dependencies between resources so they're deployed in the correct order.
* Apply access control to all services because RBAC is natively integrated into the management platform.
* Apply tags to resources to logically organize all the resources in your subscription.
* Clarify your organization's billing by viewing costs for a group of resources that share the same tag.

## Azure regions and availability zones
Resources are created in regions, which are different geographical locations around the globe that contain Azure datacenters. Azure is made up of datacenters located around the globe. When you use a service or create a resource such as a SQL database or virtual machine (VM), you're using physical equipment in one or more of these locations. These specific datacenters aren't exposed to users directly. Instead, Azure organizes them into regions. 

### Azure regions
A region is a geographical area on the planet that contains at least one but potentially multiple datacenters that are nearby and networked together with a low-latency network. Azure intelligently assigns and controls the resources within each region to ensure workloads are appropriately balanced. When you deploy a resource in Azure, you'll often need to choose the region where you want your resource deployed.

### Azure availability zones
You want to ensure your services and data are redundant so you can protect your information in case of failure. When you host your infrastructure, setting up your own redundancy requires that you create duplicate hardware environments. Azure can help make your app highly available through availability zones.

### Azure region pairs
Availability zones are created by using one or more datacenters. There's a minimum of three zones within a single region. It's possible that a large disaster could cause an outage big enough to affect even two datacenters. That's why Azure also creates region pairs. Because the pair of regions is directly connected and far enough apart to be isolated from regional disasters, you can use them to provide reliable services and data redundancy. Some services offer automatic geo-redundant storage by using region pairs.

Additional advantages of region pairs:
* If an extensive Azure outage occurs, one region out of every pair is prioritized to make sure at least one is restored as quickly as possible for applications hosted in that region pair.
* Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage.
* Data continues to reside within the same geography as its pair (except for Brazil South) for tax- and law-enforcement jurisdiction purposes.
