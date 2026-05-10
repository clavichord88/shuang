<link rel="stylesheet" href="assets/style.css">
---
title: Azure
---

[Home](index.md) | [About](about.md) | [Projects](projects.md) | [Contact](contact.md)

---

# Microsoft Fabric
Fabric is a unified software-as-a-service (SaaS) platform where all data is stored in a single open format in OneLake. All analytics engines in the platform can access OneLake, ensuring scalability, cost-effectiveness, and accessibility from anywhere with an internet connection.

### OneLake
OneLake is Fabric's centralized data storage architecture that enables collaboration by eliminating the need to move or copy data between systems. OneLake unifies your data across regions and clouds into a single logical lake without moving or duplicating data. OneLake is built on Azure Data Lake Storage Gen2 (ADLS Gen2) and supports various formats, including Delta, Parquet, CSV, and JSON. For tabular data, the analytical engines in Fabric write data in delta-parquet format and all engines interact with the format seamlessly.

Shortcuts are references to files or storage locations within OneLake or external data sources, such as Azure Data Lake Storage, Amazon S3, or Dataverse. Shortcuts allow you to access existing data without copying it, ensuring data consistency and enabling Fabric to stay in sync with the source.

### Workspaces
In Microsoft Fabric, workspaces serve as logical containers that help you organize and manage your data, reports, and other assets. They provide a clear separation of resources, making it easier to control access and maintain security.

Each workspace has its own set of permissions, ensuring that only authorized users can view or modify its contents. This structure supports team collaboration while maintaining strict access control for both business and IT users. Workspaces allow you to manage compute resources and integrate with Git for version control. You can optimize performance and cost by configuring compute settings, while Git integration helps track changes, collaborate on code, and maintain a history of your work.


You can learn more **[About me](../about.md)** or **[Contact me](../contact.md)**.
