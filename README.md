# 🛒 AtoZ E-Commerce Data Platform Modernisation  
### Databricks Lakehouse Pilot Project

---

## Client Background

**AtoZ** is a rapidly growing US-based e-commerce company selling consumer products across multiple categories. As the business expanded, both the **volume** and **velocity** of transactional data increased significantly, placing strain on the company’s existing data infrastructure.

What initially worked for a smaller organization began to fail at scale, leading to delayed analytics, frozen dashboards, and limited visibility into daily business performance. To address these challenges, AtoZ initiated a **Databricks Lakehouse pilot** to modernise its data platform and validate a scalable alternative to its legacy ETL architecture.

---

## The Scalability Crisis

### Nature of the Crisis

The issue was not poor code quality, but a **platform-level scalability limitation**.

AtoZ relied on Python-based ETL pipelines distributed across AWS services, including Lambda, Glue, and EC2. As data volumes grew, these pipelines struggled to handle large-scale transformations, becoming a bottleneck for analytics and reporting workloads.

### Business & Operational Impact

The technical limitations led to tangible business consequences:

- ❌ Dashboards freezing during peak usage  
- ⏱️ Delayed daily reports are impacting leadership decisions  
- 📉 Marketing teams are unable to access prior-day data on time  
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

The pilot introduces **Databricks as a centralised compute and analytics layer**, replacing fragmented ETL logic with a unified Lakehouse architecture.

### End-to-End Data Flow

![AtoZ Databricks Architecture](https://github.com/ayadaziz/Databricks_Ecom_Repo/blob/main/databricks_architecture.png)

---

## Data Architecture Strategy

This project follows the Medallion Architecture to enforce data quality boundaries and improve scalability.

![AtoZ Pipeline](https://github.com/ayadaziz/Databricks_Ecom_Repo/blob/main/building-data-pipelines-with-delta-lake-120823.png)


##  Analysis & Insights  

This analysis evaluates AtoZ’s 2025 commercial performance using analytics-ready Gold-layer datasets built on Databricks. The objective is to identify **revenue drivers, demand dynamics, channel efficiency, and geographic risk**, and translate insights into **actionable business recommendations**.

---

## Executive Summary

**Overall performance in 2025 shows short-term volatility rather than structural decline.**  
Revenue fluctuations are primarily driven by **changes in order volume**, not pricing. Mobile emerges as the highest-value channel, while customer demand is **highly concentrated geographically**, presenting both growth opportunities and concentration risk.

**Key conclusions:**
- Revenue declines are **volume-driven**, not AOV-driven  
- Mobile consistently outperforms the website in customer value  
- Customer base is heavily concentrated in India  
- Regional revenue efficiency varies significantly  

---

## 1. Sales Revenue Trend (Monthly – 2025)

### Key Insight  
Monthly revenue peaked in **August**, declined sharply in **September**, and recovered in **October**, indicating a **temporary demand dip rather than a sustained downturn**.

- August: ₹621.7M (peak)  
- September: ₹574.9M (lowest)  
- October: ₹618.1M (recovery)

### Evidence  
```md
![Monthly Sales Revenue – 2025](<img width="775" height="280" alt="image" src="https://github.com/user-attachments/assets/a89e7981-cb1e-410f-a390-f15945893bbc" />
)

