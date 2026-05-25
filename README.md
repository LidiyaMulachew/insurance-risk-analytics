# End-to-End Insurance Risk Analytics & Predictive Modeling

## Overview

This project is an end-to-end data science pipeline built on historical auto insurance data from South Africa.

It follows industry-standard practices including:
- Exploratory Data Analysis (EDA)
- Statistical Hypothesis Testing
- Machine Learning for Predictive Modeling
- Data Version Control (DVC) for reproducibility

The goal is to:
- Understand insurance risk patterns
- Segment customers by risk level
- Test statistical differences across groups
- Build predictive models for claim severity
- Support risk-based premium pricing decisions

---

## Objectives

### 1. Exploratory Data Analysis (EDA)
- Understand dataset structure and distributions
- Identify missing values, outliers, and anomalies
- Analyze relationships between:
  - Risk vs income
  - Claims vs premium
  - Risk by age, region, and vehicle type
  - Zip code-based risk patterns

---

### 2. Hypothesis Testing
Statistical testing was performed to validate risk differences:

- Risk differences across provinces
- Risk differences across zip codes
- Margin (profit) differences across zip codes
- Risk differences between genders

Techniques used:
- T-tests
- Statistical significance (p-value < 0.05)

---

### 3. Predictive Modeling
Machine learning models were built to predict insurance claim severity:

Models used:
- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

Evaluation metrics:
- RMSE (Root Mean Squared Error)
- R² Score

A risk-based pricing framework was designed using predicted claim severity.

---

### 4. Business Insights
Key insights from the analysis:
- Certain customer segments show significantly higher claim risk
- Risk varies strongly by region and vehicle characteristics
- Customer attributes can be used to estimate expected loss
- Enables dynamic, data-driven insurance pricing strategy

---

### 5. Data Version Control (DVC)
This project uses DVC to ensure reproducibility and auditability.

#### Features:
- Raw and cleaned datasets tracked separately
- Data versioning enabled for all experiments
- Reproducible pipeline for all analysis steps
