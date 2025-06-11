# 📉 Simple Linear Regression Analysis

This project was developed as part of **Course 2 of the Google Advanced Data Analytics Certificate**. It simulates a real-world business case where a data analyst builds and evaluates a simple linear regression model to explore the relationship between a single predictor and a response variable.

---

## 📌 Project Overview

The objective of this activity is to perform and evaluate a simple linear regression using a real-world dataset. This involves checking assumptions, fitting the model, and interpreting key metrics such as R-squared, coefficients, and residuals.

**Main questions explored:**

- Does a linear relationship exist between the chosen variables?
- How strong is this relationship?
- Can we use this model to make reliable predictions?

---

## 🧪 Development Process

### 1. Data Preparation

- Loaded dataset into a Pandas DataFrame.
- Checked for missing values and corrected data types.
- Selected appropriate numeric variables for regression modeling.

### 2. Model Development

- Ran a simple linear regression model using `statsmodels` and `scikit-learn`.
- Calculated coefficients, intercepts, and R-squared values.
- Visualized the regression line and residuals.

### 3. Model Evaluation

- Checked linear regression assumptions:
  - Linearity
  - Homoscedasticity
  - Normality of residuals
- Evaluated model performance using:
  - R-squared
  - P-values
  - Confidence intervals

---

## 📊 Key Insights

- A significant linear relationship was found between the independent and dependent variable.
- The R-squared value indicates that the model explains a large proportion of variance.
- Residual plots confirmed that the assumptions of linear regression were reasonably met.
- The slope coefficient suggests a meaningful relationship: as X increases, Y increases/decreases on average.

---

## 📁 Project Files

- `Activity_Run_simple_linear_regression-.ipynb`  
  → Contains model setup, training, and visualizations.

- `Activity_Evaluate_simple_linear_regression-2.ipynb`  
  → Includes residual analysis, assumption checks, and model interpretation.

---

## 🛠 Tools Used

- Python
- pandas
- matplotlib
- seaborn
- scikit-learn
- statsmodels
- Jupyter Notebook

---

This project showcases the end-to-end process of performing and evaluating a simple linear regression model, reinforcing essential skills for data analysts working with predictive modeling.
