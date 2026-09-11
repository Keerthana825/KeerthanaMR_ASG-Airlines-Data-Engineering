# ASG Airlines – End-to-End Data Engineering & Business Intelligence Project

## 📌 Project Overview

This project presents an end-to-end data engineering and business intelligence solution for ASG Airlines.

The objective is to process and analyze airline operational flight data, identify data quality issues, perform meaningful business analysis, and develop an interactive Power BI dashboard for decision-making.

The project uses Databricks for data processing, SQL for business analysis, and Power BI for visualization.

---

## 🎯 Objectives

- Process and clean raw airline operational data.
- Identify and handle data quality issues.
- Standardize airline, route, duration, and flight-related information.
- Perform exploratory and business-oriented analysis using SQL.
- Prepare a reliable dataset for business intelligence reporting.
- Develop an interactive Power BI dashboard.
- Generate insights related to airlines, routes, flight duration, and overnight operations.

---

## 🏗️ Project Architecture

```text
Raw Airline Dataset
        │
        ▼
   Data Ingestion
        │
        ▼
     Databricks
        │
        ▼
Data Cleaning & Transformation
        │
        ▼
 Processed Dataset
        │
        ├───────────────┐
        ▼               ▼
      SQL          Power BI
    Analysis       Dashboard
        │               │
        └───────┬───────┘
                ▼
        Business Insights