# azure-medallion-data-platform
End-to-end Azure data engineering project using Azure Synapse Pipelines and Azure Databricks implementing Medallion Architecture (Bronze, Silver, Gold) for scalable data processing and analytics.

Data Source (Excel / CSV)
        │
        ▼
Azure Data Lake Storage (Raw Zone)
        │
        ▼
Azure Synapse Pipeline (Orchestration)
        │
        ▼
Azure Databricks (Spark Processing)
        │
        ▼
Medallion Architecture

Bronze Layer
Raw Data Tables

Silver Layer
Cleaned & Transformed Data

Gold Layer
Aggregated Analytics Tables
        │
        ▼
Power BI / Analytics
