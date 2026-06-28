# 🎵 End-to-End Azure Data Engineering Project | Spotify Data Pipeline

## 📌 Project Overview

This project demonstrates the design and implementation of a modern **end-to-end Azure Data Engineering pipeline** using Microsoft Azure services and Azure Databricks.

The solution follows the **Medallion Architecture (Bronze → Silver → Gold)** to ingest, transform, govern, and curate Spotify streaming data for analytics. The pipeline leverages metadata-driven orchestration, incremental data loading, Delta Lake, and Slowly Changing Dimension (SCD Type 2) processing to simulate a real-world enterprise data platform.

The project showcases how raw operational data can be transformed into trusted, analytics-ready datasets using scalable cloud-native technologies.


## 🎯 Business Problem

Organizations receive continuous data from operational systems, but raw data alone cannot support reliable reporting or analytics.

Common challenges include:

- Manual ETL processes
- Poor data quality
- Lack of centralized storage
- No historical tracking of dimension changes
- Difficulty managing incremental data loads
- Limited governance and data lineage
- Inefficient pipelines that reload complete datasets

To address these challenges, this project implements a scalable Azure-based data platform capable of automatically ingesting, transforming, and maintaining historical data while preparing trusted datasets for downstream analytics.

## 💡 Solution Overview

The solution automates the complete data engineering lifecycle.

1. Azure Data Factory orchestrates metadata-driven incremental data ingestion.
2. Azure SQL Database serves as the operational source system.
3. Azure Data Lake Storage Gen2 stores data using the Medallion Architecture.
4. Azure Databricks processes raw data using PySpark and Auto Loader.
5. Delta Live Tables implement SCD Type 2 for Gold layer dimensions.
6. Unity Catalog provides centralized governance and metadata management.
7. Azure Logic Apps send automated email notifications when pipeline failures occur.

The final Gold layer contains curated business-ready datasets suitable for reporting, dashboards, and advanced analytics.


# 🏗️ Solution Architecture

> **Architecture Diagram**

<p align="center">
    <img src="images/architecture.png" width="95%">
</p>

---

## 🔄 End-to-End Workflow

```text
Azure SQL Database
        │
        ▼
Azure Data Factory
(Metadata Driven Pipeline)
        │
        ▼
Azure Data Lake Storage Gen2
        │
        ▼
Bronze Layer
(Raw Data)
        │
        ▼
Azure Databricks
(PySpark + Auto Loader)
        │
        ▼
Silver Layer
(Cleansed & Standardized)
        │
        ▼
Delta Live Tables
(Auto CDC + SCD Type 2)
        │
        ▼
Gold Layer
(Business Ready Data)
        │
        ▼
Power BI / Analytics
```

---

# ☁️ Azure Resources

The complete solution is deployed on Microsoft Azure using multiple managed cloud services.

<p align="center">
    <img src="images/resource-group.png" width="95%">
</p>

### Azure Resources Used

| Azure Service | Purpose |
|--------------|---------|
| Azure SQL Database | Source system for Spotify datasets |
| Azure Data Factory | Metadata-driven orchestration and incremental ingestion |
| Azure Data Lake Storage Gen2 | Centralized data lake implementing Medallion Architecture |
| Azure Databricks | Distributed data processing using PySpark |
| Unity Catalog | Centralized governance and metadata management |
| Delta Live Tables | Gold layer processing and SCD Type 2 implementation |
| Azure Logic Apps | Email notifications for pipeline failures |
| GitHub | Version control and source code management |

---

# ⭐ Project Highlights

- Metadata-driven ETL pipeline
- Incremental Data Loading
- Medallion Architecture
- Azure Data Factory Orchestration
- Azure Databricks
- PySpark Transformations
- Auto Loader
- Delta Lake
- Delta Live Tables
- Slowly Changing Dimension (SCD Type 2)
- Unity Catalog
- Logic App Integration
- GitHub Version Control

---

# 📑 Table of Contents

- Project Overview
- Business Problem
- Solution Overview
- Solution Architecture
- Technology Stack
- Repository Structure
- Azure Resources
- Dataset
- Azure Data Factory
- Azure Data Lake Storage
- Azure Databricks
- Medallion Architecture
- Silver Layer Transformations
- Gold Layer (SCD Type 2)
- Delta Live Tables
- Unity Catalog
- Pipeline Monitoring
- Screenshots
- Challenges
- Skills Demonstrated
- Future Improvements
- How to Run
- Acknowledgements
- License

  
