# Credit Risk Analysis & Customer Segmentation

## Overview

This project analyzes customer credit behavior using the UCI Credit Card dataset. The objective is to identify meaningful customer segments and predict default risk using a combination of exploratory data analysis (EDA), clustering techniques, and machine learning models.

Additionally, an interactive Power BI dashboard was developed to support data-driven insights and facilitate business decision-making.

---

## Objectives

- Perform exploratory data analysis to understand customer financial behavior  
- Segment customers based on credit characteristics using clustering techniques  
- Apply dimensionality reduction (PCA) for visualization and feature optimization  
- Build a predictive model to estimate default payment risk  
- Develop an interactive dashboard for data visualization and business insights  

---

## Technologies Used

- Python (Pandas, NumPy, Scikit-learn)
- Machine Learning
- Clustering (K-Means)
- Dimensionality Reduction (PCA)
- Logistic Regression
- Power BI
- Data Visualization

---

## Project Structure
```
credit-risk-customer-segmentation
│
├── README.md
│
├── data
│ └── uci_credit_card_dataset.csv
│
├── notebooks
│ └── credit_risk_analysis.ipynb
│
├── dashboards
│ └── credit_risk_dashboard.pbix
│
└── images
├── pca_clusters.png
├── correlation_matrix.png
└── dashboard_preview.png

```
---

## Data Preparation & Processing

The dataset was initially loaded into Power BI (Power Query) for data cleaning and transformation. Key preprocessing steps included:

- Verification of missing values and duplicates (none found)
- Removal of unnecessary columns such as ID
- Data type adjustments for numerical consistency

The cleaned dataset was then processed in Python:

- Standardization using **StandardScaler (Z-score normalization)**
- Ensuring all features contributed equally to the analysis
- Preparation for clustering and modeling

---

## Exploratory Data Analysis (EDA)

EDA was conducted to understand the distribution and relationships between variables.

Key insights included:

- Strong correlations among billing amount variables
- Variability in payment behaviors across customers
- Indicators of potential financial risk patterns


---

## Customer Segmentation (Clustering)

Customer segmentation was performed using **K-Means clustering**.

### Steps:

- Data normalization using StandardScaler  
- Dimensionality reduction using **Principal Component Analysis (PCA)**  
- Selection of optimal number of clusters (k = 3)  
- Assignment of each customer to a cluster  

PCA was also used to visualize customer segmentation in a reduced 2D space.

### Outcome:

- Identification of distinct customer groups
- Differentiation based on credit usage and payment behavior
- Insights into varying levels of financial risk across clusters

---

## Predictive Modeling

A **Logistic Regression model** was developed to predict the probability of default payment.

### Model Features:

- Target variable: `default_payment_next_month`
- One-hot encoding applied to categorical variables:
  - SEX, EDUCATION, MARRIAGE
  - Payment history variables (PAY_0 to PAY_6)
  - Cluster labels
- Train-test split: 80/20
- Class imbalance handled using `class_weight='balanced'`

### Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- AUC (ROC Curve)

---

## PCA-Based Feature Engineering

Due to strong multicollinearity among billing features (`BILL_AMT1` to `BILL_AMT6`), PCA was applied:

- First two principal components captured most of the variance
- These components replaced original billing features in a second model

### Result:

- Reduced multicollinearity
- Slight decrease in model performance
- Indicates that some predictive information was lost during dimensionality reduction

---

## Power BI Dashboard

An interactive dashboard was developed to visualize key insights and support business decisions.

### Dashboard Features:

- Customer segmentation analysis
- Credit limit and payment behavior comparison
- Default risk indicators
- Cluster-based insights

<img width="1296" height="732" alt="image" src="https://github.com/user-attachments/assets/023b61bd-383a-4373-ad7f-29a3f93faa00" />


---

## Key Insights

- Customer segmentation reveals distinct financial behavior patterns  
- Certain clusters exhibit higher default risk  
- Billing variables show strong correlation, indicating redundancy  
- Logistic regression provides a solid baseline for default prediction  
- PCA helps reduce dimensionality but may reduce predictive performance  

---
