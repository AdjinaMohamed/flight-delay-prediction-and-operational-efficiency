# 📚 Data Dictionary  
## Flight Delay Prediction & Operational Efficiency Analysis

This file describes all variables used in the project.  
(TBD fields will be filled after EDA.)

---

## 1. flights_2024 / flights_2025

| Column Name | Description | Example | Notes |
|------------|-------------|---------|-------|
| flight_id | Unique flight identifier | TBD |  |
| airline | Airline operating the flight | TBD |  |
| origin | Departure airport code | MUC |  |
| destination | Arrival airport code | FRA |  |
| scheduled_departure | Planned departure time | TBD | Convert to datetime |
| actual_departure | Real departure time | TBD | May have missing |
| scheduled_arrival | Planned arrival time | TBD |  |
| actual_arrival | Real arrival time | TBD |  |
| delay_departure | Departure delay in minutes | TBD | target engineering |
| delay_arrival | Arrival delay in minutes | TBD |  |
| status | On time / delayed / cancelled | TBD | Clean needed |

---

## 2. airport_traffic_2024 / 2025

| Column Name | Description | Example |
|-------------|-------------|---------|
| date | Calendar date | 2025-01-01 |
| airport | Airport code | MUC |
| flights_total | Number of flights that day | TBD |
| passengers | TBD | optional |

---

## 3. airports.csv

| Column Name | Description |
|-------------|-------------|
| iata_code | Airport code |
| name | Airport name |
| city | City |
| country | Country |
| latitude | Decimal latitude |
| longitude | Decimal longitude |

---

## 4. runways.csv

| Column Name | Description |
|-------------|-------------|
| airport | Airport code |
| runways | Number of runways |
| length | Longest runway length |
| surface | Runway surface type |

---

## 5. flights_bavaria_2025.csv

| Column Name | Description |
|-------------|-------------|
| Same as flights dataset | Focus on Bavaria region |

---

## 6. Stakeholder_Punctuality.xlsx

| Column | Description |
|--------|-------------|
| kpi_name | KPI name |
| formula | Definition |
| stakeholder | Airline / airport |

---

*More fields will be added after EDA.*
