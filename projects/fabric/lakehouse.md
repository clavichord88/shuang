## <link rel="stylesheet" href="assets/style.css">

## title: Describe lakehouse features and capabilities

[Home](index.md) | [About](about.md) | [Projects](projects.md) | [Contact](contact.md)

---

A lakehouse organizes data into two main areas: Tables and Files.

- Tables folder: This folder contains Delta Lake tables that provide structured, queryable data.
- Files folder: This folder stores raw or semi-structured data files in their native format.

This separation lets you maintain both raw data (for compliance or reprocessing) and structured tables (for analytics) within the same lakehouse. You can process files using Spark notebooks or Dataflows Gen2, then load the results into tables for querying and reporting.
At the heart of a lakehouse are Delta Lake tables. Delta Lake is an open-source storage layer that brings reliability to data lakes. When you create a table in a lakehouse, the data is stored in Delta format in the underlying OneLake storage. Each Delta table consists of Parquet data files plus a transaction log that tracks all changes. This architecture enables both batch and streaming workloads to work reliably with the same data.

---

You can learn more **[About me](../about.md)** or **[Contact me](../contact.md)**.
