# Notebooks

This directory contains the main Jupyter Notebook used for the analysis, modeling, and customer segmentation process.

---

## File

- **code.ipynb**

---

## Contents

The notebook includes the complete analytical workflow:

### 1. Data Loading and Preprocessing

- Data import
- Feature selection
- Standardization using StandardScaler
- Preparation for clustering and modeling

---

### 2. Exploratory Data Analysis (EDA)

- Statistical summaries
- Correlation analysis
- Identification of key patterns in financial behavior


---

### 3. Predictive Modeling

- Logistic Regression model
- One-hot encoding of categorical variables
- Train-test split (80/20)
- Model evaluation using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - AUC

---

### 4. PCA Feature Engineering

- PCA applied to billing variables (`BILL_AMT1` to `BILL_AMT6`)
- Dimensionality reduction
- Comparison between original and PCA-based models

---

## Purpose

The notebook demonstrates the end-to-end data science workflow, from data preprocessing to advanced modeling and evaluation, providing insights into customer credit behavior and default risk.
