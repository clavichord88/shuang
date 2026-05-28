## <link rel="stylesheet" href="assets/style.css">

## title: OneLake

[Home](index.md) | [About](about.md) | [Projects](projects.md) | [Contact](contact.md)

---

The OneLake catalog helps you discover and browse data assets across your entire Fabric tenant. Think of it as a searchable inventory of all the data in OneLake. The catalog makes it possible to find relevant data even when you don't know exactly where it's stored.

The catalog also provides governance and security capabilities. OneLake integrates with Microsoft Purview for data governance. You can classify data, apply sensitivity labels, and track data lineage. Access controls determine who can read or modify data, providing enterprise-grade controls to protect your data. OneLake uses Delta Lake as the default table format, which stores data in open Parquet files.

The catalog respects access permissions, which keeps sensitive data secure while enabling discovery of available resources. This permission-based visibility means different team members see different catalogs based on their roles.

Endorsement helps others find trusted content. There are three endorsement levels:

- Promoted: The item is ready for sharing. Any user with write permissions can promote an item.
- Certified: The item meets your organization's quality standards. Only authorized reviewers can certify items.
- Master data: The item is an authoritative source of truth for core organizational data like customer lists or product codes. Only authorized reviewers can apply this label.

### Sematic models

When you find semantic models in the catalog, you can explore and connect to them for reporting. Semantic models contain prebuilt relationships, calculations, and business metrics that make it easier to create reports.

### Discover streaming data

The Real-Time hub is the centralized catalog for discovering and managing streaming data across Microsoft Fabric. While the OneLake catalog shows batch data stored in lakehouses and warehouses, the Real-Time hub displays eventstreams and KQL tables that are actively running in your organization. Streaming data often flows into eventhouses, which are containers that hold one or more KQL databases. These databases store time- or event-based events and support fast querying by using Kusto Query Language (KQL).

You can learn more **[About me](../about.md)** or **[Contact me](../contact.md)**.
