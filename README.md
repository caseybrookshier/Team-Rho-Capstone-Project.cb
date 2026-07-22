# Predicting State-Level Inpatient Suicide-Related Admissions with Google Trends

**Team:** Team Rho  
**Authors:** J. Casey Brookshier, Brendan Collari  
**Tools:** Python, Jupyter Notebook, pandas, scikit-learn, XGBoost, SHAP  

---

## 📌 Project Overview

This project evaluates whether suicide- and crisis-related Google Trends search activity can predict future state-level inpatient psychiatric admissions.

The primary research question is:

> Which suicide- and crisis-related Google search terms provide the most accurate leading indicators of state-level inpatient psychiatric admissions one year later?

The project combines online search behavior, healthcare utilization, healthcare capacity, and population data to improve prediction of future mental health service demand.

---

## 🧠 Analytical Focus Areas

- Suicide and crisis-related Google Trends indicators
- State-level inpatient psychiatric utilization forecasting
- Healthcare capacity adjustment
- Population-normalized admission rates
- Predictive modeling and feature importance analysis

---

## 📊 Data Sources

- **Google Trends**
  - State-level search interest for terms such as:
    - "suicidal thoughts"
    - "suicide hotline"
    - "self harm"
    - "suicide prevention"

-**HCUP Data (Healthcare Utilization Outcome)**
   - Retrieve state-level Mental Health/Substance Use inpatient admission data.

- **U.S. Census Bureau Population Estimates**
  - State population normalization for admission rate calculations

---

## 🤖 Modeling Approach

Predictive models evaluate whether lagged Google Trends features improve one-year forecasts of suicide-related inpatient  admissions.

Models include:

- Multiple Linear Regression (baseline)
- Random Forest
- XGBoost
- PCA (feature reduction)
- Hierarchical clustering (state similarity analysis)
- SHAP feature importance

Performance metrics:

- RMSE
- MAE
- R²

---

## 📁 Repository Structure

```text
Team-Rho-Capstone-Project/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
├── src/
├── figures/
├── reports/
├── README.md
├── requirements.txt
└── .gitignore