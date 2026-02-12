IaaS (Infrastructure as a service)- Inclue services that are basically computing services, storage services, and networking
services. Genrally make it equivalent to owning a data center. So Azure Virtual Machine is IaaS as it is a server with nothing install until you actually install your own software or third-party software, make it do something. 
Vms are paid by the second. In Vms you get lot of choices in CPU speed, RAMS and etc. You also get azure storage with upto 5Pb of capacity and can also be configured as data lake.
Virtual Networking are also provided which is free where ingree (inbound data ) is free but egress (data going out) is not free
though you get 5 GB of egress bandwidth for free

PaaS ( Platform as a Service)- Now in this cloud provider provide more than the IaaS like scaling, redunancy, secuirty, updates, patching, maintenance etc . In this azure procide us with the platform to run our apps like webapp we can run it but we dont have access to the vm its running.

SaaS( Software as a Service)- These are basically full fledged apps - cloud apps like office 365, One drive, Skype. In this application are ready to use.

"As a Service" = it itself means that you can rent it for a short time as your wish, no commitment and pay for what you use

Serverless - It doesnt mean there is no servers but you don't manage the servers but only handle writing and running the code.
No need to pre purchase or reserve the resource.
Example 1=
SQL Database Options- Azure has multiple sql database options-
        - DTU-based - Fixed Performance level (S1,S2,etc.) paying monthly.
        - vCore-based - You Choose CPU, memory and storage require precison usually if you kind of have a databse but you                           dont use it and from this you can save some money.
        - Serverless - Auto-scales CPU & Memory based on usage. It auto scales from 0.5 to 80 vCores. You are charged per                          vCore-second and storage used. It can pause when idle, cutting costs entirely. 
Example 2= 
Azure function = First 1 million execution are free. After that you pay per execution and execution time. Azure handles scaling automatically

With all these advantage the disadvantage of serverless are that -
    -No access or insights to the underlying hardware. No idea of CPU type or memory running
    -Cant predict the cost as its based on consumption
    -Same things like SQL that go to pause or shutdown when idle so to resume it will take some seconds that means it will not be hot avail for service cosnumers.

-----Serverless means -
     - focus on code not the infrastructure. 
      -  Pay for consumption no need for estimation of cost.
        - its ideal for event driven or low usage workloads.

Azure serverless offering - Functions, Container apps, kubernetes, SQL database , Cosmos DB

