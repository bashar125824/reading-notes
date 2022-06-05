# Azure Storage

***The Azure Storage platform is Microsoft's cloud storage solution for modern data storage scenarios. Azure Storage offers highly available, massively scalable, durable, and secure storage for a variety of data objects in the cloud. Azure Storage data objects are accessible from anywhere in the world over HTTP or HTTPS via a REST API. Azure Storage also offers client libraries for developers building applications or services with .NET, Java, Python, JavaScript, C++, and Go. Developers and IT professionals can use Azure PowerShell and Azure CLI to write scripts for data management or configuration tasks. The Azure portal and Azure Storage Explorer provide user-interface tools for interacting with Azure Storage.***

## Benefits of Azure Storage

***Azure Storage services offer the following benefits for application developers and IT professionals:***

- **Durable and highly available** 
- **Secure**
- **Scalable**
- **Managed**
- **Accessible**

## Azure Storage data services

***The Azure Storage platform includes the following data services:***

- **Azure Blobs** : ***A massively scalable object store for text and binary data. Also includes support for big data analytics through Data Lake Storage Gen2.***

- **Azure Files** : ***Managed file shares for cloud or on-premises deployments.***

- **Azure Queues** : ***A messaging store for reliable messaging between application components.***

- **Azure Tables** : ***A NoSQL store for schemaless storage of structured data.***

- **Azure Disks** : ***Block-level storage volumes for Azure VMs.***

![IMG](https://wakeupandcode.com/wp-content/uploads/2019/08/storage-icons.png)


# What is Azure Blob storage ?

***Azure Blob storage is a feature of Microsoft Azure. It allows users to store large amounts of unstructured data on Microsoft’s data storage platform. In this case, Blob stands for Binary Large Object, which includes objects such as images and multimedia files. These are known as unstructured data because they don’t follow any particular data model.***

***Azure Blob storage is more focused on common storage purposes. In other words, it  includes objects which personal users would be used to storing, such as photos, videos, and documents. On an enterprise level, the amount of these files, as well as log files and backups is considerably higher, hence the need for Azure. ***

***Blob storage for an organization, for example, would mean keeping backups of previous versions of a site and its content and images, which would need to be accessible from different locations. By using Azure data storage, a company can make this material easier and quicker to access compared to it being kept on a single-location server.***


***With Azure Blob storage, the files (photos, videos, training documents, etc.), which are known as blobs, are put in containers which function similar to directories. These are then linked to the storage account. When creating the address to give access to a file in Azure data storage, it will simply join the storage account and the location of the blob. The address will be in a .net format.***


![IMG](https://miro.medium.com/max/1400/0*PYSS__o2sYQBYgKd.png)


## Uses of Blob storage :

- **Serving images or documents directly to a browser.**
- **Storing files for distributed access.**
- **Streaming video and audio.**
- **Writing to log files.**
- **Storing data for backup and restore, disaster recovery, and archiving.**
- **Storing data for analysis by an on-premises or Azure-hosted service.**


***Users or client applications can access objects in Blob storage via HTTP/HTTPS, from anywhere in the world. Objects in Blob storage are accessible via the Azure Storage REST API, Azure PowerShell, Azure CLI, or an Azure Storage client library. Client libraries are available for different languages, including:***

- **.NET**
- **Java**
- **Node.js**
- **Python**
- **Go**
- **PHP**
- **Ruby**


## Blob storage resources

***Blob storage offers three types of resources:***

- **The storage account** : ***provides a unique namespace in Azure for your data. Every object that you store in Azure Storage has an address that includes your unique account name. The combination of the account name and the Blob Storage endpoint forms the base address for the objects in your storage account.***

- **A container in the storage account** : ***A container organizes a set of blobs, similar to a directory in a file system. A storage account can include an unlimited number of containers, and a container can store an unlimited number of blobs.***

- **A blob in a container** : ***There is three types :***

1. **Block blobs** : ***store text and binary data. Block blobs are made up of blocks of data that can be managed individually. Block blobs can store up to about 190.7 TiB.***

2. **Append blobs** : ***are made up of blocks like block blobs, but are optimized for append operations. Append blobs are ideal for scenarios such as logging data from virtual machines.***

3. **Page blobs** : ***store random access files up to 8 TiB in size. Page blobs store virtual hard drive (VHD) files and serve as disks for Azure virtual machines.***




