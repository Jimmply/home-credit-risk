# 🏦 Home Credit Default Risk — Credit Risk Modeling

## 📌 Project Overview
This project aims to predict the probability that a loan applicant will default on a loan using the **Home Credit Default Risk** dataset from Kaggle.

Credit risk modeling is a critical task for financial institutions. Accurate predictions help lenders:

* minimize financial losses  
* optimize approval strategies  
* offer loans to reliable clients  
* improve portfolio risk management  

This project is built as an **end-to-end, production-style data science workflow**, not just a Kaggle submission.

---

## 🎯 Business Objective
Develop a machine learning model that estimates:

> **What is the probability that a client will have payment difficulties?**

This is a **binary classification problem** where:

* `TARGET = 1` → client with payment difficulties (default)
* `TARGET = 0` → client repays the loan

The primary evaluation metric is:

> **AUC (Area Under the ROC Curve)**  
which is suitable for imbalanced datasets.

---

## 📂 Project Structure

credit/
│
├── data/ # Raw data (not uploaded to GitHub)
│
├── notebooks/
│ ├── 01_business_understanding_and_eda_application_train.ipynb
│
├── outputs/
│ └── missingness_summary.csv
│
└── README.md


---

## 📊 Day 1 — Exploratory Data Analysis (Application Table)

### ✔ Data Understanding
* The dataset contains client financial, demographic, and loan application information.
* The target variable is **highly imbalanced**, which reflects real-world credit risk.

### ✔ Missing Values Analysis
* Several features contain a high percentage of missing values.
* This will require:
  * imputation strategies
  * feature engineering
  * or feature removal

### ✔ Key Risk Drivers Explored
We performed an initial analysis of:

* Age
* Income
* Credit amount
* Annuity
* Education level
* Income type
* Family status

### ✔ Initial Observations
*(Will be updated as the project progresses)*

Examples:

* Clients with higher credit exposure tend to show higher default risk.
* Default rate varies across income and education categories.
* Strong class imbalance confirms the need for robust validation using AUC.

---

## 🧠 Key Skills Demonstrated

* Business-driven problem framing
* Reproducible project structure
* Data cleaning strategy design
* Missing value auditing
* Risk-oriented exploratory analysis
* Feature type assessment

---

## ⚙️ Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Jupyter Notebook
* Scikit-learn *(upcoming)*
* LightGBM *(upcoming)*

---

## 🚀 Next Steps

### 🔹 Baseline Model
* Stratified train/validation split
* Missing value imputation
* One-hot encoding
* Baseline Logistic Regression / LightGBM
* Cross-validation with AUC

### 🔹 Feature Engineering (Core of the Project)
We will aggregate information from:

* bureau
* previous_application
* POS_CASH_balance
* installments_payments
* credit_card_balance

to build **client-level behavioral risk features**.

### 🔹 Model Explainability
* Feature importance
* SHAP values
* Business interpretation of risk drivers

---

## 📈 Project Goal

This project is designed to demonstrate **real-world, job-ready data science skills**, including:

* working with large relational datasets
* building end-to-end ML pipelines
* translating data into business insights

---

## 📎 Dataset

Kaggle Competition:  
**Home Credit Default Risk**
