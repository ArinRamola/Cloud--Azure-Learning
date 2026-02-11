Regions - Areas around the world where azure has set of datacenter not necessarily in every country or only one set of datacenter 
in one country. Each set has atleast has 3 datacenter. Also they make sure that as per the country policy data can or cannot leave 
the country(data residency concept) like cannada azure data cannot leave the country while brazil azure data can leave the country
Also all the datacenter region do have pairs but qatar is the sole region with no pair so you cant use the Geo-Redundant Storage 
Option but do support availabilty zone.
There are 60+ region but not necessarily allowed to use.

Availabilty Zones- these are physically separate location within a region. They are miles apart from each other and no way relaint
on each other in any other way. They have their own resources. Not every region has availability zone like canada east. Basically 
needed if you want to have a backups and since they are in a same region so their transer speed is less than 5ms.
Three type of availabilty zone Region
               - Zonal Services - is basically letting a customer choose their own specific availability zone for their services.
               - Zone-Redundant Services - Automatically deployed across the zones for you. You dont have to configure it.
               - Always Available zone - Services that always run on or are not in any region called "non- regional services"

Resource hierarchy = Resources(lowest) -> Resource groups -> Subscription -> Management Group.

Resource -  its basically used to to define the services of azure such as your VMs, Storage account or Databases and they can be 
created many diffrent ways sucha as  Azure Portal, CLI, PowerShell, ARM template, etc. Each resouce has a name given by you. 
Sometimes it needs to be unique and their geographic place where they are running.

Resource Group - Its a logical grouping of resources. its is associated with a region but that doesnt block you to put resource
from diffrent location. Resource group should have a similarities don't put resource with no relation to a resource group 
together. Permissions can also be applied on a resource group level. 

Subscription - its in basic its a billing unit. every resource exist in a single subscription and their bill is incurred in it.
A payment method is also incurred in that subscription. It also has administrative boundary for governance, compliance and 
access control and operate at subscription level. Plans - free plan - $200 credit, pay as you go billed to credit card, Enterprise
Agreement -EA or in some plan such as student plan.
A user can have multiple subscription through Role based Access control. Mostly used by companies to separeate diffrent departemnts
or separate by geography.

Management Groups -> A centralized point to control all the subscriptions. Highly use by organisations and at top of hierarchy 
there is Root Management Group which control or create these management groups.
Along witb a Root mangement group you can have upto maximum 5 management groups.


