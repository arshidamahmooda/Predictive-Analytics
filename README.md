# README - Multiple Linear Regression

## Overview
This script implements **Multiple Linear Regression** to predict **horsepower** based on various features of cars. The dataset used contains multiple numerical and categorical variables, which are preprocessed before training the regression model.

---

## File Description

### **multiple_linear_regression.py**
- Loads the dataset (`cars.csv`).
- Performs **data preprocessing**, including:
  - Handling missing values
  - Removing duplicates
  - Encoding categorical variables using one-hot encoding
  - Detecting and handling outliers
  - Feature scaling using `StandardScaler`
  - Checking for multicollinearity using **Variance Inflation Factor (VIF)**
- Builds a **Multiple Linear Regression Model** using `LinearRegression()` from Scikit-Learn.
- Evaluates model performance using:
  - **Mean Squared Error (MSE)**
  - **R-squared (R²) Score**
- Visualizes:
  - **Correlation Matrix** using Seaborn
  - **Actual vs Predicted Horsepower** scatter plot
  - **Regression Line** for better understanding

---

## Requirements
Ensure the following Python libraries are installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels scipy
```

---

## Usage
Run the script using:
```bash
python multiple_linear_regression.py
```
Make sure to update the dataset path (`cars.csv`) if needed.

---

## Model Interpretation
The regression equation follows this format:
```
Horsepower = Intercept + (Coef1 * Feature1) + (Coef2 * Feature2) + ...
```
Where:
- `Intercept` is the model's bias term.
- `Coef1, Coef2, ...` are the feature coefficients indicating their importance.

---

## Notes
- The script automatically detects and handles **multicollinearity**, **outliers**, and **categorical features**.
- Feature selection is done based on **VIF values** to remove highly correlated variables.
- The model is trained using an 80-20 **train-test split**.

---

## Author
Arshida Mahmooda
