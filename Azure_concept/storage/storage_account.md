### Azure storage account

*  An Azure storage account is a secure account that gives you access to services in Azure Storage. Your storage account provides the unique namespace for your storage resources.

* A storage account name should be unique across all existing storage account names in Azure

### Types of Storage accounts

Azure Storage provides three types of storage accounts. Each type support different features and has its own pricing model

![](../images/3.png)

### Types of performance tiers
* Standard performance tiers are backed by magnetic drives and provides low cost per GB. They are bestfor applications that are bestcfor bulk storage or infrequently accessed data

* Premium storage performance are backed by solid state drives and offers consistency and low latency performance. They can only be used with Azure virtual machine disks, and are best for I/O intensive workload such as databases.

### Storage account access tiers

* **Azure storage** offers different storage tiers which allow you to store Blob object data in the most costeffective manner

* **Premium storage** (preview) provides high performance hardware for data that is accessed frequently.

* **Hot storage**: is optimized for storing data that isaccessed frequently. Cool storage is optimized for storing data that is infrequently accessed and stored for at least 30 days.

* **Archive storage** is optimized for storing data that is rarely accessed and stored for at least 180 days withflexible latency requirements (on the orderofhours).

### Azure storage replication

Azure Storage replication copies your data so that it is protected from planned and unplanned events ranging from transient hardware failures, network or power outages, massive natural disasters, and so on.

![](../images/storage-replication.png)

### Storage account endpoints
* Every object that you store in Azure Storage has an address that includes your unique account name. The combination of the account name and the Azure Storage service endpoint forms the endpoints for your storage account.

* For example, if your general-purpose storage account is named mystorageaccount, then the default endpoints for that account are

* Blob storage: http://mystorageaccount.blob.core.windows.net 
* Table storage: http://mystorageaccount.table.core.windows.net 
* Queue storage: http://mystorageaccount.queue.core.windows.net 
* Azure Files: http://mystorageaccount.file.core.windows.net