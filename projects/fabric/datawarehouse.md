## <link rel="stylesheet" href="assets/style.css">

## title: Data warehouse in Fabric

[Home](index.md) | [About](about.md) | [Projects](projects.md) | [Contact](contact.md)

---
A Fabric data warehouse is a fully managed, enterprise-scale relational database built on OneLake. It provides full transactional T-SQL capabilities, including DDL statements (CREATE, ALTER, DROP) and DML statements (INSERT, UPDATE, DELETE, MERGE), with full ACID compliance for data consistency.
Data is stored in open Delta format on OneLake, which means other Fabric workloads can access the same data without duplication. You use T-SQL to create tables, load data, build views and stored procedures, and perform transformations, all within a familiar SQL experience.

#### Model data in a warehouse
Without data modeling, every consumer has to figure out which tables relate to each other, write their own aggregation logic, and guess at column meanings. Data modeling solves this problem by embedding structure, business logic, and documentation directly into the warehouse. In a Microsoft Fabric warehouse, you prepare data for clarity, define relationships between tables, standardize access through views and measures, and publish semantic models for reporting. These modeling choices affect every downstream experience, including T-SQL queries, Power BI reports, and AI-driven natural language analytics.

---

You can learn more **[About me](../about.md)** or **[Contact me](../contact.md)**.
