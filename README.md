# 🛒 AtoZ E-Commerce Data Platform Modernization  
### Databricks Lakehouse Pilot Project

---

## Client Background

**AtoZ** is a rapidly growing US-based e-commerce company selling consumer products across multiple categories. As the business expanded, both the **volume** and **velocity** of transactional data increased significantly, placing strain on the company’s existing data infrastructure.

What initially worked for a smaller organization began to fail at scale—leading to delayed analytics, frozen dashboards, and limited visibility into daily business performance. To address these challenges, AtoZ initiated a **Databricks Lakehouse pilot** to modernize its data platform and validate a scalable alternative to its legacy ETL architecture.

---

## The Scalability Crisis

### Nature of the Crisis

The issue was not poor code quality, but a **platform-level scalability limitation**.

AtoZ relied on **Python-based ETL pipelines** distributed across AWS services such as Lambda, Glue, and EC2. As data volumes grew, these pipelines struggled to handle large-scale transformations, becoming a bottleneck for analytics and reporting workloads.

### Business & Operational Impact

The technical limitations led to tangible business consequences:

- ❌ Dashboards freezing during peak usage  
- ⏱️ Delayed daily reports impacting leadership decisions  
- 📉 Marketing teams unable to access prior-day data on time  
- 🛠️ High maintenance overhead due to fragmented ETL logic  
- 💰 Limited cost transparency and inefficient scaling  

Leadership identified this as a **strategic data platform problem**, not a short-term engineering issue.

---

## Pilot Objective

Instead of a full migration, leadership approved a **controlled pilot project** to validate Databricks against three success criteria:

1. **Performance**  
   Distributed Spark processing must outperform legacy Python ETL jobs.

2. **Adoption**  
   The platform should be intuitive enough for engineers and analysts to onboard quickly.

3. **Roadmap Alignment**  
   The solution must be:
   - Scalable (supporting any data volume)
   - Agile (easy infrastructure upgrades or downgrades)
   - Unified (data engineering, analytics, and AI in one workspace)

---

## High-Level Architecture

The pilot introduces **Databricks as a centralized compute and analytics layer**, replacing fragmented ETL logic with a unified Lakehouse architecture.

### End-to-End Data Flow

```text
Customers
   ↓
E-Commerce Application (OLTP)
   ↓
On-Prem Relational Database
   ↓
Python Data Extraction
   ↓
Amazon S3 (Raw Storage)
   ↓
Databricks (ETL, Processing, Data Warehouse)
   ↓
BI Dashboards & Business Users

---

## Architecture Diagram

[![AtoZ Databricks Architecture]([./architecture.png](https://github.com/ayadaziz/Databricks_Ecom_Repo/blob/main/legacy_architecture.png))](https://github.com/ayadaziz/Databricks_Ecom_Repo/blob/main/legacy_architecture.png)








