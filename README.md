# Improving Commercial Property Fire-Peril Loss Cost Modelling
### GLMs and Gradient Boosting

**Course:** CIND820 - Big Data Analytics Project - W2026
**Name:** Debra Allen
**Student Number:** 500358053
**Supervisor:** Ceni Babaoglu, PhD

---

!Python
!scikit-learn
!pandas
!Status
!Course
!Institution
!Jupyter

---

## Project Overview

This repository contains the code and initial results for the CIND820 Big Data Analytics Project titled:
> **Improving Commercial Property Fire-Peril Loss Cost Modelling with Generalized Linear Models and Gradient Boosting**

The objectvie of this project is to evaluate and compare traditional acturial modelling approaches (Tweedie GLMs) with modern machine-learning methods (Gradient Boosting) for predicting the commercial property fire-peril loss cost using a real world dataset.

The project emphasizes:
- Actuarial appropriate modelling choices
- Reproducible data science workflows
- Clear documentation and interpretability
- Empirical comparison of GLMs vs machine-learning models

---

## Dataset

**Source:** Kaggle - *Liberty Mutual Group - Fire Peril Loss Cost*

Has 105,450 commercial insurance records
Has over 300 predictor variables (numberic and categorical)
Target variable: `target` (fire-peril loss cost)

The data shows:
- Extreme **zero-inflation**
- Strong **right skewness**
- Heavy tailed loss serverity

The characteristics require the use fo Tweedie GLMs and flexible non-linear models.

---

## Methodology Summary

### 1. Exploratory Data Analysis
- Descriptive Statistics
- Loss cost distribution analysis
- Missing data analysis
- Correlation anaylsis
- Visualization of extreme skewness and sparsity

### 2. Data Preparation
- Type of conversion and validation
- Median imputation for numerical variables
- Mode imputation for categorical variables
- Standardization of numeric predictors
- One-hot encoding of categorical predictors
- Train-test split with no data leakage

### 3. Modelling Approaches
- **Tweedie GLM**
  - Compound Poisson-Gamma distribution
  - Actuarial standard for loss cost modelling
- **Gradient Boosting Regressor**
  - Captures non-linear effects and interactions
  - Used as a machine-learning benchmark

### 4. Model Evaluation
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Coefficient of Determination (R^2)
- Side-by-side comparison and visualization

---

## Key Findings

- Fire-peril loss cost is extremely difficult to predict due to a large number of zero losses.
- The Tweedie GLM slightly outperforms Gradient Boosting in baseline testing.
- Gradient Boosting does not automatically outperform standard actuarial models in sparse insurance data.
- Model structure and distributional assumptions are critical in insurance applications.

---

## How to Run Code

1. Clone the repository:
   ```bash
   git clone https://github.com/uni-Deb7943/TMU-CIND820.git

2. Install required packages
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn

3. Dataset included in the repository
   ```bash
   https://github.com/uni-Deb7943/TMU-CIND820.git

4. Run the code:
   - 01_EDA_and_Data_Analysis.ipynb
   - 02_Data_Preparation.ipynb
   - 03_Tweedie_GLM_Model.ipynb
   - 04_Gradient_Boosting_Model.ipynb
   - 05_Model_Comparison.ipynb
