Predicting Health Service Utilization with Google Trends
Team Rho

Course: DSE6311 Capstone Project

Team Members

Casey Brookshier 
Brendan Collari 
Project Overview

The objective of this project is to investigate whether Google search activity can be used as a leading indicator of future mental health service utilization within the United States.

Specifically, this project seeks to answer the following research question:

Which categories of Google search activity provide the most accurate leading indicators of state-level mental health service utilization one year later?

Rather than evaluating individual search terms alone, this project groups related Google searches into broader thematic categories (e.g., symptoms, treatment, financial stress, and substance use) and evaluates their predictive ability using statistical and machine learning models.

Objectives
Collect state-level Google Trends search data.
Obtain historical mental health utilization data from SAMHSA.
Incorporate provider capacity and demographic variables from HRSA Area Health Resource Files.
Develop baseline and machine learning prediction models.
Compare model performance using standard evaluation metrics.
Identify which Google search categories are the strongest predictors of future mental health service utilization.
Data Sources
Google Trends

Measures public interest in mental health-related search categories.

https://trends.google.com/trends

SAMHSA MH-CLD (Mental Health Client-Level Data)

Provides mental health service utilization data.

https://www.samhsa.gov/data/data-we-collect/mh-cld-mental-health-client-level-data/datafiles/2013-2024

HRSA Area Health Resource Files (AHRF)

Provides healthcare workforce, provider capacity, and demographic information.

https://data.hrsa.gov/topics/health-workforce/nchwa/ahrf

Methodology

The analysis will be conducted using a state-year dataset created by merging Google Trends, MH-CLD, and AHRF data.

The target variable is state-level mental health utilization rate:

Utilization Rate = (Mental Health Clients / State Population) × 100,000

Google Trends search terms will be grouped into thematic categories, aggregated by state and year, and lagged so that search activity during year t predicts utilization during year t + 1.

Model development will include:

Multiple Linear Regression (baseline model)
Random Forest
XGBoost
Feature importance analysis using SHAP values

Model performance will be evaluated using:

RMSE (Root Mean Squared Error)
MAE (Mean Absolute Error)
R² (Coefficient of Determination)
Repository Structure
Team-Rho-Capstone-Project/

├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── src/
│
├── figures/
│
├── reports/
│
├── README.md
├── requirements.txt
└── .gitignore
Software

The project is developed primarily in Python using Jupyter Notebooks.

Major packages include:

pandas
NumPy
Pytrends
scikit-learn
statsmodels
XGBoost
LightGBM
SHAP
matplotlib
seaborn
Plotly
MLflow

Google Colab may be used for additional computational resources during model training.

Expected Outcomes

This project will evaluate whether Google search behavior provides reliable leading indicators of future mental health service utilization. If successful, the results may help healthcare organizations and policymakers improve staffing, planning, and resource allocation through earlier identification of changing service demand.