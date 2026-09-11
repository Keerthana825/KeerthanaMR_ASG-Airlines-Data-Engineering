# ASG Airlines – Data Cleaning and Transformation

## 📌 Overview

The raw airline dataset contained several inconsistencies that needed to be addressed before performing business analysis and creating the Power BI dashboard.

Data cleaning and transformation were performed using Databricks with Python and PySpark-based processing.

---

## 1. Initial Data Inspection

The raw dataset was first inspected to understand:

- Number of records
- Number of columns
- Column names
- Data types
- Missing values
- Duplicate records
- Invalid values
- Unknown categories
- Inconsistent schemas

The initial inspection helped identify the major data quality problems.

---

## 2. Schema Normalization

The raw data contained unnecessary trailing columns generated during data ingestion.

These columns included fields similar to:

```text
_c7
_c8
_c9
_c10