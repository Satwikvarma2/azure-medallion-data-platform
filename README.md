# Azure Medallion Data Platform

## Description
This project demonstrates an **end-to-end Azure Data Engineering pipeline** built using **Azure Synapse Pipelines** and **Azure Databricks** implementing the **Medallion Architecture (Bronze, Silver, Gold)**.

The system ingests raw retail datasets (Excel/CSV), stores them in **Azure Data Lake Storage**, and processes them using **Databricks Spark workloads** orchestrated through **Synapse Pipelines**. The data is transformed across Bronze, Silver, and Gold layers to create reliable and analytics-ready datasets for reporting and business insights.

This project simulates a **modern enterprise data platform** used in many organizations for scalable data ingestion, transformation, and analytics.

---

## Architecture Diagram

Aggregated Analytics Tables
        │
        ▼
Power BI / Analytics

            Data Source
          (Excel / CSV Files)
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
                   │
      ┌────────────┼────────────┐
      ▼            ▼            ▼
   Bronze        Silver        Gold
  (Raw Data)  (Cleaned Data) (Business Tables)

                   │
                   ▼
            Analytics / BI Tools
             (Power BI / SQL)
