# Munich Airport Delay Intelligence  
Operational Analytics & KPI Framework (EDDM)

This project analyzes flight delays at Munich Airport (EDDM) with the goal of building an operational delay intelligence framework combining flight schedules, traffic volume, and weather context.

The focus is on descriptive and diagnostic analytics: identifying delay patterns, seasonal effects, airline-level differences, and operational stress indicators, and presenting them through a KPI-driven Tableau dashboard.

---

## Business Context

Munich Airport is a major European hub with complex traffic dynamics. Delays are influenced by traffic load, airline operations, weather conditions, and airport capacity constraints.

This project reflects the type of analytics work performed by airport operators or aviation performance teams, where the goal is transparent, explainable operational insights.

---

## Analytical Scope

The project focuses on:
- Delay distribution analysis by hour, weekday, and season
- Airline-level punctuality comparison
- Traffic volume versus delay relationships
- Descriptive analysis of weather context
- KPI design for operational monitoring

---

## Key Performance Indicators

- On-time performance (threshold-based)
- Average departure and arrival delay
- Delay rate by airline
- Delay rate by hour of day
- Seasonal delay intensity matrices
- Traffic volume versus delay indicators

---

## Project Structure

```text
munich-airport-delay-intelligence/
├─ README.md
├─ .gitignore
├─ notebooks/
│  └─ 01_muc_delay_analysis.ipynb
├─ src/
│  ├─ data_prep.py
│  ├─ kpi_calculation.py
│  └─ utils.py
├─ data/
│  ├─ raw/
│  ├─ processed/
│  └─ external/
├─ sql/
│  └─ kpi_queries.sql
├─ tableau/
│  └─ muc_delay_dashboard.twbx
└─ reports/
   └─ findings_muc_delay.md
