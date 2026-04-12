# Processed Data

This directory contains the cleaned and transformed dataset used for analysis and modeling.

---

## File

- **credit_processed_clusters.xlsx**

---

## Description

The processed dataset was generated after applying data cleaning, transformation, and feature engineering steps to the original dataset.

Key preprocessing steps include:

- Removal of unnecessary columns (e.g., ID)
- Verification of missing values and duplicates
- Data type standardization
- Feature scaling using StandardScaler (Z-score normalization)
- Assignment of customer clusters using K-Means

---

## Additional Features

Compared to the raw dataset, this version includes:

- Normalized numerical variables
- Cluster labels representing customer segments
- Features prepared for machine learning models

---

## Purpose

The processed dataset is used for:

- Clustering analysis
- Predictive modeling (logistic regression)
- Visualization and dashboard development

---

## Notes

- This dataset is derived from the raw data and should not be modified manually
- All transformations are documented in the project notebook
- Ensures consistency between analysis, modeling, and visualization components

This dataset represents the final analytical version of the data used throughout the project.
