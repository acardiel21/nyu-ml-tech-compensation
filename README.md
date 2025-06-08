# Tech Salaries Data Analysis and Regression Modeling

This project investigates compensation patterns in the 2017 U.S. tech industry using a dataset of 62,000+ self-reported salaries. It was completed as part of NYU's Fundamentals of Machine Learning course, with a focus on regularization, predictive modeling and data cleaning.

## Objectives
- Predict total yearly compensation using linear and regularized regression models
- Assess the predictive strength of individual features
- Evaluate fairness in salary data by investigating potential gender disparities
- Classify high vs. low earners using logistic regression

## Data Preprocessing
- Handled missing values and dropped salary-related predictors where required
- Encoded categorical variables such as gender, education level, and location
- Standardized numeric features (e.g., age, SAT score, GPA)
- Explored skewness in salary distribution and used median-based binning for classification

## Modeling Techniques

### Multiple Linear Regression
- Fitted a full model and individual simple models for comparison
- Assessed feature importance using R²
- Found “Years of Experience” to be the strongest single predictor

### Ridge Regression
- Tuned lambda across values to minimize RMSE
- Showed identical results to OLS due to low multicollinearity in data

### Lasso Regression
- Explored model sparsity and feature selection
- No predictors shrunk to zero; Lasso mirrored Ridge and OLS results

### Gender Pay Gap Analysis
- Built logistic models to predict gender from salary alone vs. with all features
- Found no significant model difference; suggests other variables influence classification

### High vs. Low Salary Classification
- Labeled salaries based on median income ($174k)
- Trained logistic regression model on demographic and academic predictors
- Achieved moderate performance (AUC: 0.73, AP: 0.72)

## Tools & Libraries
- Python (Pandas, NumPy, scikit-learn, Matplotlib)
- Models: Linear Regression, Ridge, Lasso, Logistic Regression
- Evaluation: R², RMSE, ROC AUC, Precision, Recall, Confusion Matrix

`Cardiel_Tech_Salaries.ipynb` — Main Jupyter notebook with code

`Tech_Salaries.pdf` — Full write-up and analys

---
