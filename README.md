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
  Actuarial appropriate modelling choices
  Reproducible data science workflows
  Clear documentation and interpretability
  Empirical comparison of GLMs vs machine-learning models

---

## Dataset

**Source:** Kaggle - *Liberty Mutual Group - Fire Peril Loss Cost*

Has 105,450 commercial insurance records
Has over 300 predictor variables (numberic and categorical)
Target variable: `target` (fire-peril loss cost)

The data shows:
  Extreme **zero-inflation**
  Strong **right skewness**
  Heavy tailed loss serverity

The characteristics require the use fo Tweedie GLMs and flexible non-linear models.
