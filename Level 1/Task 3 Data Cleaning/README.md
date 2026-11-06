# Airbnb Data Cleaning – Oasis Infobyte Internship

## Project Overview
This project focuses on cleaning and preparing the New York City Airbnb Open Data dataset. The objective is to identify missing values, check duplicate records, detect unusual prices, and improve data quality.

## Dataset Information
- **Dataset:** NYC Airbnb Open Data (2019)
- **Original Records:** 48,895
- **Columns:** 16
- **Source:** [Kaggle – NYC Airbnb Open Data](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning Steps
1. Loaded and inspected the Airbnb dataset.
2. Checked dataset dimensions, column names, and data types.
3. Identified missing values using Pandas.
4. Visualized missing values using a heatmap.
5. Replaced missing listing names and host names with "Unknown".
6. Converted `last_review` into datetime format.
7. Checked duplicate records.
8. Detected price outliers using the IQR method.
9. Investigated zero-price listings and removed 11 records with zero prices.
10. Validated and exported the cleaned dataset.

## Outlier Analysis
- Q1: $69
- Q3: $175
- IQR: $106
- Upper limit: $334
- Detected price outliers: 2,972

Unusual prices were investigated but retained because expensive listings may represent genuine properties.

## Before and After Comparison

| Metric | Before | After |
|---|---:|---:|
| Total Rows | 48,895 | 48,884 |
| Total Columns | 16 | 16 |
| Duplicate Rows | 0 | 0 |
| Zero Price Records | 11 | 0 |
| Missing Names | 16 | 0 |
| Missing Host Names | 21 | 0 |

## Project Structure
```text
Task 3 Data Cleaning/
│
├── dataset/
│   └── AB_NYC_2019.csv
│
├── notebook/
│   └── Data_Cleaning.ipynb
│
├── Output/
│   └── cleaned_airbnb_data.csv
│
└── README.md
```

## Output
The cleaned dataset is saved as:

`cleaned_airbnb_data.csv`

## Conclusion
The Airbnb dataset was inspected, cleaned, and validated. Missing listing and host names were handled, zero-price records were removed, and unusual prices were investigated. The cleaned dataset is ready for further analysis.

## Internship
Oasis Infobyte – Data Analytics Internship

**Task:** Level 1 – Task 3: Data Cleaning