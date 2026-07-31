# Drug Shortage Analytics & Prediction

## Project Overview

This project analyzes drug shortages in the United States using data from the U.S. Food and Drug Administration (FDA) Drug Shortage Database.

The goal is to identify key drivers of shortages, predict shortage duration and risk, and support proactive decision-making for healthcare stakeholders such as hospitals, regulators, and supply chain teams.

## Business Problem

Drug shortages can disrupt patient care, delay treatments, and increase operational costs. This project explores how data analytics can help improve visibility into shortage patterns and support proactive planning.

## Dataset

**Source:** FDA Drug Shortage Database / OpenFDA

The dataset includes:
- drug name
- manufacturer
- dosage form
- therapeutic category
- shortage status
- initial posting date
- update date

Each row represents a shortage event rather than a unique drug, so preprocessing and feature engineering were required.

## Feature Engineering

Key engineered features include:

- **Shortage Duration:** measures how long a shortage lasts
- **Long Shortage:** binary classification for shortages lasting 1000 days or more
- **Risk Level:** Low, Medium, or High based on shortage duration
- **Manufacturer Count:** number of manufacturers associated with each drug
- **Therapeutic Category Count:** number of therapeutic categories per drug

## Methods

- Data cleaning and preprocessing
- Exploratory Data Analysis
- Feature engineering
- Classification modeling
- Regression modeling
- Random Forest feature importance
- Power BI dashboard development

## Models Used

| Model | Task |
|---|---|
| Logistic Regression | Classification |
| Random Forest Classifier | Classification |
| Linear Regression | Regression |
| Random Forest Regressor | Regression |
| Gradient Boosting Regressor | Regression |

## Model Results

| Model | MAE | R² |
|---|---:|---:|
| Linear Regression | 720.96 | 0.403 |
| Gradient Boosting Regressor | 500.09 | 0.687 |
| Random Forest Regressor | 385.80 | 0.736 |

Best model: **Random Forest Regressor**

## Key Insights

- Manufacturer count is the strongest predictor of shortage duration
- Injectable dosage forms are associated with longer shortages
- Shortage behavior is non-linear
- Predictive analytics can support early risk identification

## Dashboard

The Power BI dashboard includes:

1. **Overview:** current state of shortages
2. **Drivers:** key shortage factors
3. **Predictions:** predicted duration and risk levels

Add dashboard screenshots here.

## Recommendations

- Strengthen supplier diversification for high-risk drugs
- Prioritize monitoring of injectable and complex dosage forms
- Use predictive procurement and planning strategies
- Build coordinated data-driven decision systems

## Tools Used

- Python
- Pandas
- Scikit-learn
- Power BI
- Excel
- Jupyter Notebook