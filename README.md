# Safe Haven: Predictive Analytics for Homelessness Resource Allocation
> **An end-to-end data science framework designed to forecast county-level homelessness trends and optimize social service distribution.**

## 📌 Context & Impact
This project was originally developed as the **Lead Challenge Architecture** for the **UTA Datathon 2025**. I researched, engineered, and synthesized the core datasets to create a "real-world" predictive modeling task. The framework was utilized by over 10+ teams to benchmark machine learning performance and policy-driven insights.

## 📊 The Data Engineering Challenge
Real-world socioeconomic data is rarely clean or centralized. To build this project, I integrated three heterogeneous data streams to create a unified 7-year longitudinal view of California's landscape:

1. **Homelessness Demographics (2017–2023):** County-level longitudinal data covering age, race, and gender.
2. **Healthcare Utilization Logs:** Granular hospital encounter data for homeless vs. non-homeless populations, including mental health and primary care shortage flags.
3. **Fiscal Allocation Profiles:** State-level funding data used to correlate resource injection with population shifts.

## 🛠️ Technical Workflow
### 1. Data Orchestration & Cleaning
* Developed a robust pipeline to handle missingness across 50+ California counties.
* Standardized disparate temporal granularities (Fiscal Year vs. Calendar Year) into a single analytical dataframe.

### 2. Exploratory Data Analysis (EDA)
* Identified the "Hospitalization-to-Homelessness" ratio as a leading indicator for county-level vulnerability.
* Visualized demographic shifts showing an aging homeless population (65+) in specific urban clusters.

### 3. Machine Learning & Forecasting
* **Baseline:** Established a Linear Regression baseline for 2024 forecasts.
* **Advanced Models:** Implemented **Random Forest** and **XGBoost** to capture non-linear relationships between healthcare shortages and homelessness spikes.
* **Evaluation:** Utilized Mean Absolute Error (MAE) and a custom 1000-point optimization rubric to validate model reliability.

## 📁 Repository Structure
* `/data`: Curated datasets synthesized from CA DHS and NCHE.
* `/notebooks`: `End_to_End_Analysis.ipynb` contains the full preprocessing and modeling pipeline.
* `/documentation`: Technical "Pocket Book" and "Whitepaper" detailing the methodology provided to stakeholders.

## 🚀 Key Insights for Policy
* **Shortage Correlation:** High mental health shortage flags in rural counties showed a stronger correlation with recidivism in homelessness than simple funding gaps.
* **Forecasting:** The model identified three specific "High-Need" counties where hospital utilization predicts a 15% spike in homelessness for the 2024-25 cycle.

---
**Author:** Zecil Jain
**Role:** Lead Challenge Developer (UTA Datathon '25) | Data Scientist
