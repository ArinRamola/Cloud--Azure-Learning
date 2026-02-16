Cloud Computing - is essentially a rental service where yiu an rent services such as servers, storage and etc. In Azure there are more than 1000 services.
On premisis responsibilty - physical security, network security, operating system patches, network and firewall settings, Application settings, Authentication platform, User Accounts, Data
cloud responsibilty(IAS) - physical security, network security
cloud responsibilty(PAS)- physical security, network security, operating system patches
cloud responsibility(SAS)-  physical security, network security, operating system patches, network and firewall settings, Application settings

Public Cloud -    The public cloud is defined as computing services offered by the third party providers over the public internet making them available them to anyone who want to use or purchase them.  
 - Public cloud focuses on operational expenditure as the cost, which means it's a regular monthly charge that you can deduct from your income to make your profits in the public cloud.
 - Microsoft Azure owns the hardware.
 - It's open to the general public, although they do a good job of protecting your data and protecting your environments from others.
 - The scalability is massive. It's possible that you will never be able to fill an Azure storage account.

Private Cloud - The privare cloud is defined as computing services offered by the internet or the private internal network and only selected users instead of the general public.(even if provided by third party its still build solely to you)
- the core value is speed, cost and efficiency with the private cloud.
-  Those are often upfront expenses or contractual obligations for money that has to come out. Sometimes you can't deduct those from your income. It has to be deprecated.
-  You own the hardware.
-  Access is definitely restricted.
-  Scalability is limited.
-  It's very difficult to get a new server added to your network Which can be time consuming and expensive.
-  You do get the control, the security and all.

Hybrid Cloud - Combines a private and public cloud environment by keeping the sensitive workloads  in your pricate cloud while taking advantage of public cloud scalability for less critical workload.
- It's a combination of OpEx and CapEx.
- It is controlled by both you and Microsoft Azure in terms of ownership and also in terms of access.
- You get the flexibility of owning the hardware, but also being able to scale massively into the cloud.
- And the core value is flexibility and control.

Cost
- based on geographical region
- Operating system SKU/License
- Instance size
- Disk Type/Size
- bandwidth
- backup storage
- Api choices
- optional dedicated gateway
- no. of operation per second
- etc so many of the services are free

Pricing -
- Pay how long it run for resources such as compute like vm instances
- Storage is paid by GB by month can be around 0.02$ per month and outbound traffic is paid while inbound is free
- pay for operation - such as read write and delete or like pay per message or pay per query to database etc. usually very cheap
- Azure Pricing calculator- used to estiamte the cost of your these services.

SLA (Service Level Agreement) - The uptime percent of a cloud service like for 95% SLA the yearly downtime would be 18d 6hr 17m 27s and as for a 99% it would be 3d 15h 39m 29s and as for one with 99.9% would be 8h 45m 56s and last for one with 99.99% is 52m 35s.

Calculate SLA - multiply the SLA of the participating services like a app service SLA - 99.95% and Azure SQL SLA = 99.99%
Actual SLA = 99.95*99.99 = 99.94% = 5h 15m 34s annual downtime.

Advantage 
- High Availability - the uptime your system can remain operational during planned(during a upgrade or update) and unplanned outages and provide services to your clients or customers.
Planned Outage - Operating System Security patches , Application Updates or Hardware Replacement or maybe migrating to a new host provider.
Unplanned Outage- Hardware failure, Network Disruptions, Power Outages, Natural Disaster, Cyber Attacks, Software Bugs, Poor Scaling or Architecture Design.
Methods to Mitigate planned Outages- Gradual deployment Strategy (1-10-100-etc), Testing and Monitoring of employment, Easy rollback plan , Small Deployments,Frequent Deployemnts, Automation.
Methods to Mitigate unplanned Outages- Azure Built in features, Single core component (having entire application depend on any one single component), Constant Health Monitoring, Automation.

- Scalability - It allows to adapt to the changing usage patterns and handle increased traffic without requiring changes to the application code or system design.
   So what Scales a System ??? ----- 1- Vertical Scaling - Adding more resources to a single server, increase the memory or no. of cpu ----limit - 96vCPUs, 348 GB Memory
                                     2- Horizontal Scaling - Add more server to a system, No limit to Scaling, Add complexities for load balancing
   Cost Impact - add more as resource add but if load is less the code also decrease, Having a scalable system allows for a system to be a perfect size. Can be manual or automatic

- Elasticity - the ability to quickly scale up and scale down the amount of resources a system needs as per the change in demand by azure based on real-time workload. Its automatic. In this there is capacity which is always greater than the demand to make sure there is some space even and that system dont lag but this also make some waste in resource though minimum but still it is there. You can adjust it by marking the highest capacity.

- Reliability - the ability of a system to recover from failure. There can be many failures even in a well built design ex -hardware failure , network interruptions, Power Failure , large scale regional outage. Solution - Auto Scaling , Avoid Single point of failure have multiple backups, Having data in multiple region so even if one region in case goes down you can run your system through other regions, Data Backup and Replication, Montoring,

- Predictability - The ability to forecast and control the performance and behaviour of the system. Including the ability to predict future costs.
  Its needed to give confidence that the system will perform at the expected level in the future and that you won't get some crazy massive bill.
  Methods - Auto Scaling being able to to scale up and scale down gives you some control over the costs ,  load balancing gives you predictability so you can again predict the performance of a system because you can create new instances when that is in, Cost management section of the portal can predict your rest of the month bill at your current rate.

- Security - Cloud provider is one of the massive targets of hackers so cloud security go through the security audits and massive compliance certficate and provide tools to customers so that they can monitor and secure their own application or data.
  Its needed to make sure that our chosen cloud provider can secure our data from hackers
  Method- Industry standard compliance certification , microsoft security response center, Detect attacks such as DDos, Using Azure policy, Role based access control, Update management, always up to date platform services, using security services.

- Governance - The Process of defining, implementing and monitoring a framework of policies that guides an organizations cloud operation. Simply put following the rules that put company out of trouble and let company operate in a way that is valid with other governing organisation.
  Needs - So company policies are being followed in the cloud which include basic auditing and reporting as well as enforcement
  Method - Azure Policy and Blueprint allows you to ensure across all your subscriptions and all your departments that a certain minimum standards of policies, roles, resource groups, and other things are being followed , Management Groups -  allow you to manage your subscriptions and apply policies to certain groups that apply to all the subscriptions under that group, Custom roles - being able to create your own custom roles on which azure will enforce the permission that you assigned, Soft delete - that even after delete it will not completely be delted and be in a state where it can recovered.

- Managability - in two parts
               - Mangaemnt of the cloud - in this there are all the ways that cloud providers provide to mange your                          application like automation through scripting, resources through templates, auto-scaling and monitoring                     and alerts, Self healing. 
               - Managemnt in the cloud - in this you have web portal, Command line interface and scripts, APIs, Powershell
  Managability is needed so that its easy to manage the cloud and can help in cost, performance, security, and your other     priorities.
  Method - Azure Portal, CLI , Powershell, Cloud Shell, REST APIs, and other programmatic methods, monitoring and alerting    method, Autoscale, Ability to use terraform, Bicep, ARM template etc.
  
  
  




