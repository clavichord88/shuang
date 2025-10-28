<link rel="stylesheet" href="assets/style.css">
---
title: Azure
---

[Home](index.md) | [About](about.md) | [Projects](projects.md) | [Contact](contact.md)

---

# Azure Notes

### Azure Cosmos DB (PaaS, optional Serverless)
Azure Cosmos DB is a globally distributed, multi-model database service provided by Microsoft Azure. It’s designed for applications that need high performance, low latency, and global scalability.

1. Global distribution – You can replicate your data across multiple Azure regions with just a few clicks, ensuring high availability and low latency worldwide.

2. Multi-model support – Cosmos DB supports several data models:
    1. Document (using APIs like MongoDB or SQL API)
    2. Key-value (Table API)
    3. Graph (Gremlin API)
    4. Column-family (Cassandra API)
3. Automatic scaling – It can automatically scale throughput (measured in Request Units per second, RU/s) based on your app’s workload.

4. Guaranteed performance – Microsoft provides Service Level Agreements (SLAs) for latency, throughput, availability, and consistency.

5. Five consistency levels – From strong to eventual, letting you balance performance and accuracy based on your app’s needs.

##### Common Use Cases

1. Real-time personalization (e.g., recommendation systems)
2. IoT data ingestion and analytics
3. E-commerce product catalogs
4. Mobile or gaming backends with global users

### Azure Backup (PaaS)
Azure Backup is a cloud-based backup service from Microsoft Azure that helps you protect and recover your data stored in on-premises systems, Azure virtual machines (VMs), and other cloud resources. Azure Backup automatically copies (backs up) your data to the Azure cloud, so you can restore it if it’s lost, deleted, or corrupted due to hardware failure, ransomware, or human error.
##### Key Features
1. Fully managed (PaaS) — Microsoft handles infrastructure, storage, and maintenance.
2. Automatic backups — You can schedule backups daily, weekly, or monthly.
3. Multiple recovery options — Restore entire VMs, files, folders, or individual data items.
4. Long-term retention — Store backups for months or years to meet compliance needs.
5. Encryption and security — Data is encrypted in transit and at rest, with built-in ransomware protection.
6. Integration with Azure services — Works with Azure VMs, SQL databases, file shares, and even on-premises servers via the Azure Backup Agent or Azure Backup Server.

##### Common User Cases
1. Backing up Azure Virtual Machines (VMs)
2. Protecting on-premises servers or files using the cloud
3. Backing up Azure Files and SQL databases
4. Disaster recovery planning

### Azure File (PaaS)
Azure Files is a cloud file storage service in Microsoft Azure that lets you create shared network file systems — just like a traditional file server — but fully managed and hosted in the cloud. Azure Files provides shared folders that you can access using SMB (Server Message Block) or NFS (Network File System) protocols — the same ones used in Windows, macOS, and Linux.
So, it’s like having a cloud-based file server that can be mounted on multiple computers or virtual machines anywhere.
It supports synchronization between on-premises storage and Azure storage.

##### Key Features
1. Standard SMB/NFS access – Mount Azure file shares on Windows, Linux, or macOS using normal file path syntax (e.g., \\storageaccount\share).
2. Fully managed (PaaS) – No need to set up or maintain servers or disks.
3. Integration with on-premises systems – Use Azure File Sync to keep local file servers and cloud shares synchronized.
4. Scalable and durable – Built on Azure Storage, so your files are automatically replicated and protected.
5. Access control – Supports Azure Active Directory (AAD) and NTFS permissions for secure access.
6. Backups and snapshots – Supports point-in-time file recovery.

##### Common Use Cases
1. Replacing or supplementing on-premises file servers.
2. Shared file storage for Azure VMs or applications.
3. Central file repository for multiple users across locations.
4. Hybrid setups with Azure File Sync (keep frequently used files local and store backups in Azure).

### Microsoft Intune (SaaS)
Microsoft Intune is a cloud-based device and application management service that helps organizations securely manage computers, mobile devices, and apps from a central location. hink of Intune as a tool that lets IT administrators:
1. Control which devices can access company data,
2. Enforce security policies (like password or encryption rules), and
3. Remotely manage and update employee devices (Windows, macOS, iOS, Android).

##### Key Features
1. Device Management (MDM)
    - Enroll and manage company-owned or BYOD (Bring Your Own Device) devices.
    - Enforce security settings (e.g., PIN, encryption, OS updates).

2. Application Management (MAM)
    - Control how corporate apps and data are used (e.g., prevent data copy/paste).
    - Deploy or remove apps remotely.

3. Conditional Access
    - Integrates with Azure Active Directory (Azure AD) to allow only compliant devices to access corporate resources.
4. Compliance and Reporting
    - Monitor device health, compliance status, and generate reports.
5. Integration with Microsoft 365
    - Works seamlessly with Outlook, Teams, and other Microsoft apps for secure data access.

##### Common Use Cases
    - Setting up new employee laptops or phones with company apps and policies automatically.
    - Protecting company data on personal (BYOD) devices.   
    - Remotely wiping data from lost or stolen devices.
    - Ensuring all devices comply with security standards.
    
### Azure Virtual Network

### Local Network Gateway and Virtual Network Gateway

You can learn more **[About me](../about.md)** or **[Contact me](../contact.md)**.
