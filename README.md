# Comparative Analysis of Linear Regression Models with Regularization and Feature Selection

## Project Overview

This project investigates several linear regression techniques, focusing on methods for regularization and feature selection. The main approaches used in the project are:

- **Linear Regression**
- **Forward Stepwise Selection**
- **Hypothesis Testing for Regression Coefficients**
- **Ridge Regression**
- **Lasso Regression**
- **Elastic Net Regression**
- **Principal Component Analysis (PCA)**
- **Principal Component Regression (PCR)**

## Methods Overview

### 1. Forward Stepwise Selection Based on Hypothesis Testing for Regression Coefficients
- This method starts with an empty set of predictors (denoted as **S**).
- Variables are added one by one to the set based on their predictive power for the target variable (**y**).
- At each step, a variable is included if it meets the statistical significance threshold.
- The process continues until a stopping rule is satisfied (e.g., based on a p-value criterion).

### 2. Hypothesis Testing for No Effect
- Hypothesis tests are used to assess whether a predictor has a significant impact on the target variable.
- These tests evaluate the regression coefficients to decide which variables to keep or discard.

### 3. Ridge Regression, Lasso, and Elastic Net
- **Ridge Regression**: Introduces a regularization term to shrink the regression coefficients, reducing the risk of overfitting.
- **Lasso Regression**: Adds a penalty term that can drive some coefficients to zero, which leads to automatic variable selection.
- **Elastic Net**: Combines the penalties from both Ridge and Lasso, achieving a balance between selecting important features and shrinking coefficients.

### 4. Principal Component Analysis (PCA)
- PCA is a technique used to reduce the dimensionality of the dataset by transforming it into a set of linearly uncorrelated components.
- It identifies the principal directions (components) that explain the largest amount of variance in the data, which simplifies the model.

### 5. Principal Component Regression (PCR)
- PCR first applies PCA to the predictors and then fits a linear regression model using the principal components.
- This approach helps to address multicollinearity and reduces model complexity.

## Dependencies

The project requires the following Python libraries:

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas**: For data manipulation and handling.
- **NumPy**: For numerical computations.
- **Scikit-learn**: For implementing machine learning algorithms, including regression models and PCA.
- **Matplotlib**: For creating plots and visualizations.
- **Seaborn**: For enhanced statistical data visualization.
