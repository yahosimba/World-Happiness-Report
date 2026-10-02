# World Happiness Report 2016 Data Analysis

A Python-based data cleaning, imputation, and exploratory data analysis (EDA) project based on the **World Happiness Report (2016)** dataset. This repository demonstrates how to load, inspect, clean, impute missing values, and construct interactive visualizations using `pandas`, `numpy`, and `plotly`.

---

## 📌 Project Overview

This project ingests raw country-level happiness data for the year 2016, performs standardized data preprocessing, cleans up string fields and null values, converts columns to proper nullable pandas dtypes, and generates an interactive bar chart comparing key quality-of-life metrics among top-ranking countries.

Key steps in the pipeline:
1. **Data Ingestion**: Loading raw CSV data into a pandas DataFrame.
2. **Inspection**: Verifying shape, non-null counts, and data types.
3. **Data Cleaning & Standardization**:
   - Trimming whitespace from object/string columns.
   - Replacing empty strings with `NaN` values.
   - Converting DataFrame dtypes to modern pandas nullable types (`string`, `Int64`, `Float64`).
4. **Missing Value Handling**:
   - Detecting null values across all columns.
   - Imputing numeric missing values using column-level means.
5. **Data Visualization**: Creating an interactive grouped bar chart displaying **Economy (GDP per Capita)** versus **Health (Life Expectancy)** for the top 10 happiest nations.

---

## 📁 Repository Structure

```text
.
├── 2016.csv                 # Raw dataset (World Happiness 2016)
├── cleaned_2016.csv         # Standardized dataset with modern dtypes
├── final_2016_imputed.csv   # Cleaned dataset with missing value imputation
├── notebook.ipynb           # Jupyter Notebook with full analysis code
└── README.md                # Project documentation