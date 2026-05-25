# Task 4: Statistical Modeling & Risk-Based Pricing

## 1. Objective
The objective of this task is to develop predictive models for insurance claim severity and design a risk-based pricing framework that estimates expected claim costs using machine learning techniques.

---

## 2. Models Used
Three models were implemented and evaluated:

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

These models were trained to predict `TotalClaims` for policies with claims > 0.

---

## 3. Model Performance

The models were evaluated using:
- RMSE (Root Mean Squared Error)
- R² Score

The comparison results are summarized in the attached file:
`model_comparison.csv`

Key observation:
- XGBoost and Random Forest performed better than Linear Regression, indicating that non-linear relationships exist in the dataset.

---

## 4. Feature Importance Analysis

Feature importance was analyzed using tree-based models.

Key drivers of claim severity include:
- Vehicle characteristics
- Policy type
- Customer risk profile (e.g., NCD, age, region)

Full feature importance ranking is available in:
`feature_importance.csv`

---

## 5. Business Interpretation

The model suggests that insurance risk is not uniform across customers. Certain variables significantly influence claim severity.

For example:
- Higher-risk vehicles are associated with higher claim costs.
- Customers with better risk profiles (e.g., higher NCD) tend to generate lower claims.

This supports the need for **risk-based pricing**, where premiums are adjusted based on predicted claim severity.

---

## 6. Conclusion

The XGBoost model provided the best performance and is recommended for deployment in a risk-based pricing system. This model enables more accurate premium estimation and improves financial sustainability for the insurer.