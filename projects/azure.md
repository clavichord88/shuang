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
Azure Virtual Network (VNet) is the fundamental building block for private networking in Azure.

It allows Azure resources (VMs, databases, web apps, etc.) to securely communicate with each other, the internet, and on-premises networks. VNets are isolated by default — resources in one VNet cannot talk to another unless you explicitly connect them (via peering or a gateway). 

- Network Security Group: Control inbound and outbound traffic using rules (like a firewall). You use NSGs to control access and firewall rules to manage traffic flow. Which feature controls inbound and outbound traffic at the subnet or NIC level?
- Peering: Connects two VNets to allow private communication across them. Can two VNets in different regions communicate? Yes, using VNet Peering. 
- VPN Gateway: Enables secure communication between Azure and on-premises networks (hybrid connection).
- ExpressRoute: Provides a private, dedicated connection between Azure and your on-premises network — not over the internet.


### Local Network Gateway and Virtual Network Gateway

- Virtual Network Gateway (VNG): The Azure-side gateway - it represents your Azure Virtual Network (VNet) and handles traffic coming into or going out of Azure. The Virtual Network Gateway is the “door” on the Azure side.
- Local Network Gateway (LNG): The on-premises-side representation — it defines the on-premises network (your physical data center) for Azure to connect to. The Local Network Gateway is the “door” on your on-premises side.

### Azure Sphere

Azure Sphere is a secure, end-to-end IoT platform designed by Microsoft to protect connected devices - especially microcontroller-based (MCU) devices - from security threats.

It provides hardware, operating system, and cloud-based security services all in one solution.

Azure Sphere = Secure hardware (MCU) + Secure OS + Cloud security service. They Keep IoT devices up to date, Protect against hacking and malware, Ensure secure communication between devices and the cloud.

Which Azure service provides a secure, end-to-end solution for connecting, managing, and protecting IoT devices with built-in hardware, OS, and cloud-based security? Azure Sphere.

### IoT Central

It’s one of the three main IoT services you should know (along with IoT Hub and Azure Sphere). Azure IoT Central is a fully managed IoT (Internet of Things) application platform that lets you quickly connect, monitor, and manage IoT devices — without having to build the backend infrastructure yourself.

Think of it as a ready-made IoT solution (Software as a Service - SaaS) built on top of Azure IoT Hub (which is a PaaS service).
- Fully managed: Microsoft handles all infrastructure, scaling, and maintenance — you just configure and use it.
- Device management: Easily connect, monitor, and control IoT devices at scale.
- Dashboard and Analytics: Provides prebuilt dashboards to visualize data from connected devices.
- Security and Reliability: Includes built-in device authentication, role-based access, and secure communication.
- Integration: Works seamlessly with other Azure services (like Azure IoT Hub, Azure Stream Analytics, Power BI, etc.).

Your company wants to deploy an IoT solution quickly without worrying about managing cloud infrastructure. Which Azure service should you use? Azure IoT Central


### IoT Hub

Azure IoT Hub is a cloud-based Platform as a Service (PaaS) that acts as a central message hub for secure communication between IoT devices and the cloud. It’s the core messaging and management backbone for building custom IoT solutions.

- Azure IoT Hub = The messaging bridge between devices and Azure.
- Azure IoT Central = A ready-made IoT solution that actually uses IoT Hub behind the scenes.
- Azure Sphere = Secures the physical IoT devices that connect to IoT Hub.

Which Azure service provides secure, two-way communication between IoT devices and the cloud? Azure IoT Hub
Your team wants to build a custom IoT solution that handles device communication, but you’ll manage the application and visualization yourself. Which service should you use? Azure IoT Hub

### Azure Logic Apps

Azure Logic Apps is a cloud-based service that helps you automate workflows and integrate apps, data, services, and systems - both in the cloud and on-premises - without writing much (or any) code. It’s a serverless workflow automation tool - meaning Microsoft manages all the infrastructure for you.
- Automate tasks like sending emails, moving files, or posting to Teams/Slack when certain events happen.
- You build workflows visually in the Azure Portal using a drag-and-drop designer.
- Has hundreds of built-in connectors to services like Outlook, SharePoint, Twitter, SQL Server, Salesforce, and more.

Which Azure service allows you to automate workflows and integrate apps, data, and services using a visual, no-code designer? Azure Logic Apps
Your company wants to automatically send an alert email when a file is uploaded to an Azure storage account. Which Azure service can do this with minimal code? Azure Logic Apps

### Azure Blueprints

Azure Blueprints is a governance tool in Azure that helps you define and deploy a repeatable set of resources, policies, and configurations - ensuring your organization’s standards, security, and compliance are consistently applied across multiple Azure environments. Azure Blueprints = a template for creating compliant, pre-configured Azure environments.
- Standardize how resources are set up (subscriptions, resource groups, policies, etc.)
- Ensure compliance and security from the start.
- Quickly deploy governed environments for development, testing, or production.
Which Azure service allows you to define a repeatable set of governance tools such as role assignments, policies, and resource templates for consistent deployment? Azure Blueprints
Your company wants to ensure every new Azure subscription complies with organizational policies and standards. Which Azure service should you use? Azure Blueprints

### Application Insight

Azure Application Insights is a feature of Azure Monitor that helps you monitor the performance, availability, and usage of applications - both cloud and on-premises. It automatically detects performance anomalies, provides telemetry data, and helps diagnose issues in real time.

- Tracks application response times, failure rates, and performance bottlenecks.
- Gathers data such as requests, exceptions, dependencies, and page views.
- Simulates user access to check if an app or website is running properly.
- Visualize data through customizable charts, metrics, and reports in Azure Monitor or Power BI.
- Works with Visual Studio, GitHub, and Azure DevOps for continuous monitoring and troubleshooting.

Which Azure service helps developers detect issues, diagnose crashes, and monitor application performance in real time? Azure Application Insights
Which Azure service provides application telemetry, performance metrics, and failure detection for a web app? Azure Application Insights

### Azure Storage 
- Azure Blob Storage: Stores unstructured data like images, videos, backups, logs, or large binary files. Hosting images or videos for a website.
- Azure File Storage: Shared file system accessible via SMB or NFS protocol — similar to a network file share. Lift-and-shift applications that need file shares.
- Azure Queue Storage: Stores messages that applications use to communicate asynchronously. Queueing tasks between app components (e.g., background job processing).
- Azure Table Storage: Stores structured NoSQL data — key/attribute pairs. Storing metadata or configuration info.
- Azure Disk Storage: Provides persistent disks for Virtual Machines (VMs). Used as virtual hard drives for VMs.

### Azure RBAC
Azure Role-Based Access Control (RBAC) is a system that lets you manage who has access to Azure resources, what they can do, and which areas they can access. It helps organizations grant the right access to the right people - using roles instead of individual permissions. 

Which Azure feature allows you to grant users only the permissions they need to perform their job? Azure Role-Based Access Control (RBAC)

What role should you assign to a user who needs to view resources but not modify them? Reader

If a user is given Contributor access at the subscription level, what does that mean? They can manage all resources within that subscription but cannot grant access to others.

Examples of Built-in Roles: Owner, Contributor, Reader, User Access Administrator.

### Microsoft Purview

Microsoft Purview is a unified data governance and compliance solution in Azure. Microsoft Purview helps you ensure that your organization’s data is well-governed, secure, and compliant with internal and external regulations (like GDPR, HIPAA, etc.). Microsoft Purview Data Governance is for managing and cataloging data across cloud and on-prem environments. Microsoft Purview Compliance Manager is for assessing and managing compliance risks and regulatory requirements.

### fault domain

### storage redundancy options: GRS, ZRS, LRS, GZRS

### Azure B2C

### Community Cloud

### Microsoft Entra Domain Services


You can learn more **[About me](../about.md)** or **[Contact me](../contact.md)**.
