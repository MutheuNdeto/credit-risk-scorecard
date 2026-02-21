# Credit Risk Scorecard – Logistic Regression Model

## 📖 Project Overview

This project builds a credit risk classification model using logistic regression, inspired by traditional bank scorecard modeling practices.

The objective is to predict the probability of default using behavioral and demographic features.

The workflow follows regulated finance standards:

1. Data Understanding  
2. Feature Engineering  
3. Logistic Regression Modeling  
4. Model Validation (AUC, Gini, KS)  
5. Interpretation of Risk Drivers  

---

## 📊 Dataset

UCI Default of Credit Card Clients Dataset  
- 30,000 observations  
- Behavioral repayment variables  
- Credit exposure variables  
- Binary default target  

---

## 🛠 Model Approach

Model Type: Logistic Regression  
Features Used:
- `credit_limit_capped`
- `AGE`
- `delinquent_sept`

Scaling applied for numerical stability.

---

## 📈 Model Performance

| Metric | Value |
|--------|--------|
| AUC | 0.72 |
| Gini | 0.44 |
| KS Statistic | ~0.38 |

This demonstrates strong discriminatory power for a baseline model.

---

## 🔍 Key Risk Drivers

- **Delinquency in September** → Strong positive effect on default probability  
- **Credit Limit** → Higher limit associated with lower risk  
- **Age** → Small positive impact  

---

## 📂 Repository Structure

notebooks/
01_data_understanding.ipynb
02_data_cleaning.ipynb
03_modeling_scorecard.ipynb

outputs/
model_coefficients.csv
plots/roc_curve.png

requirements.txt
README.md
