# ASG Airlines – Data Engineering Architecture

## 📌 Overview

The ASG Airlines project follows an end-to-end data engineering and business intelligence architecture.

The pipeline transforms raw airline data into a cleaned analytical dataset and finally into business insights through SQL and Power BI.

---

## 🏗️ High-Level Architecture

```text
                 RAW DATA
                    │
                    ▼
            Data Ingestion
                    │
                    ▼
              DATABRICKS
                    │
          ┌─────────┴─────────┐
          ▼                   ▼
   Data Inspection       Data Quality
          │                   │
          └─────────┬─────────┘
                    ▼
          Data Cleaning
                    │
                    ▼
        Data Transformation
                    │
                    ▼
          Processed Dataset
              │           │
              │           │
              ▼           ▼
            SQL       POWER BI
          Analysis    Dashboard
              │           │
              └─────┬─────┘
                    ▼
            Business Insights