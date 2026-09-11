# ASG Airlines – Data Dictionary

## 📌 Overview

This document describes the important fields used in the ASG Airlines flight dataset.

The data dictionary provides information about the meaning, purpose, and expected data type of each field used during analysis.

---

## 📊 Dataset Fields

| Column | Description | Data Type |
|--------|-------------|-----------|
| `flight_id` | Unique identifier assigned to a flight | String |
| `airline` | Name of the airline operating the flight | String |
| `route` | Origin and destination combination | String |
| `origin` | Departure airport or city | String |
| `destination` | Arrival airport or city | String |
| `duration` | Flight duration | Numeric |
| `duration_minutes` | Flight duration converted into minutes for analysis | Integer |
| `departure_time` | Scheduled departure time | Time/String |
| `arrival_time` | Scheduled arrival time | Time/String |
| `flight_date` | Date associated with the flight | Date |
| `overnight_flight` | Indicates whether the flight operates overnight | Boolean |
| `overnight_percentage` | Percentage of flights operating overnight for a given group | Numeric |
| `total_flights` | Total number of flights | Integer |

> **Note:** The exact column names may vary depending on the final processed dataset. The definitions above describe the analytical fields used in the project.

---

## 🔑 Important Derived Fields

### Flight Duration in Minutes

Flight duration was standardized into minutes to make comparison and aggregation easier.

This field is used for:

- Average duration
- Route-level duration analysis
- Airline-level duration comparison
- Identification of abnormal duration values

---

### Overnight Flight

A derived field was created to identify flights that operate overnight.

This field is used to calculate:

- Total overnight flights
- Overnight flight percentage
- Overnight flights by airline
- Overnight flights by route

---

### Route

The route represents the combination of the flight origin and destination.

Example:

```text
BOM-CCU