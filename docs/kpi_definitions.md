# 📊 KPI Definitions  
## Flight Delay Prediction & Operational Efficiency

This document defines all operational and punctuality KPIs used in the analysis and dashboard.

---

## 1. On-Time Performance (OTP)
**Definition:**  
Percentage of flights arriving within 15 minutes of scheduled arrival.

**Formula:**  
OTP = 1 - (Delayed Flights / Total Flights)

---

## 2. Average Delay (Arrival)
**Definition:**  
Mean arrival delay across all flights.

**Formula:**  
avg_delay_arrival = sum(delay_arrival) / count(flights)

---

## 3. Peak-Hour Delay Rate
**Definition:**  
Delay rate during defined peak hours (e.g., 06–09 & 16–19).

---

## 4. Cancellation Rate
**Formula:**  
cancellation_rate = cancellations / total_flights

---

## 5. Airline Punctuality Score
Weighted score based on delay rate, cancellations, and schedule complexity.  
(To be filled after EDA.)

---

## 6. Runway Utilization
**Formula:**  
runway_utilization = flights_per_day / number_of_runways

---

## 7. Traffic vs Delay Correlation
Pearson/Spearman correlation between traffic and average delay.

(To be evaluated after EDA.)
