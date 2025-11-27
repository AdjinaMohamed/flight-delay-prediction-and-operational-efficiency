✈️ Flight Delay Prediction & Operational Efficiency Analysis (2024–2025)
End-to-end data analytics project: KPIs, Machine Learning, Tableau Dashboard
🎯 Project Overview

This project analyzes flight punctuality and airport operational performance using 2024–2025 flight, traffic, runway, and airport datasets.
It combines data engineering, KPI creation, machine learning, and visual analytics to deliver a complete airport analytics system.

The goal is to:

Build operational KPIs for stakeholders

Identify delay patterns across routes, airlines, hours, weekdays, and seasons

Engineer features from schedule, airport capacity, and traffic volume

Train a machine learning model predicting flight delays

Create a Tableau dashboard for interactive analysis

This structure mirrors real processes used by aviation analytics teams (airlines & airports).

📁 Repository Structure
data/
│── raw/               # Original datasets (2024–2025)
│── processed/         # Cleaned datasets used for modeling
│── external/          # Additional data sources

notebooks/
│── 01_data_exploration.ipynb
│── 02_feature_engineering.ipynb
│── 03_model_training.ipynb
│── 04_dashboard_prep.ipynb

src/
│── __init__.py
│── data_preparation.py
│── feature_engineering.py
│── model_training.py
│── utils.py

dashboards/
│── tableau/             # Tableau workbook
│── screenshots/         # Dashboard screenshots

docs/
│── system_design.md     # Architecture & pipeline flow
│── data_dictionary.md   # Definitions of all fields
│── model_design.md      # ML system, features, evaluation
│── kpi_definitions.md   # All punctuality & operational KPIs
│── dashboard_design.md  # Dashboard layout & logic

reports/
│── findings.pdf         # Final stakeholder report

📊 Analytical Components
1. Operational KPIs

On-time rate

Average arrival/departure delay

Cancellation rate

Airline performance ranking

Route-level punctuality

Seasonal & hourly delay patterns

Traffic vs delay correlation

Runway utilization

2. Delay Prediction Model

Target:
delay_15 = 1 if delay >= 15 minutes else 0

Features engineered:

Time: hour, weekday, month, season

Airport: number of runways, traffic load

Airline: historical punctuality score

Route: distance, origin-destination encoding

Schedule: peak-hour indicator

Models tested:

Logistic Regression

Random Forest

Gradient Boosting / XGBoost

Evaluation metrics:

Accuracy

Precision & Recall

F1-score

ROC–AUC

Feature importance + SHAP values

📈 Tableau Dashboard

(Dashboard will be added as soon as completed.)

The dashboard includes:

Delay heatmaps

Airline punctuality

Route-level performance

Seasonal patterns

Traffic-volume vs delay relationships

Cancellation overview

🧱 Tech Stack

Python: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost
Visualization: Tableau
Tools: Git, GitHub, VS Code, Jupyter Notebooks

📌 Project Status

 Repository structure created

 README initialized

 Data exploration

 Feature engineering

 Modeling

 Dashboard design

 Final report

 Publish on LinkedIn

📬 Contact

If you're a recruiter or data team interested in aviation analytics, feel free to contact me.
