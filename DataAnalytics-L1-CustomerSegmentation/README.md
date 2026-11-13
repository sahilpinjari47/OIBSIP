# Customer Segmentation Analysis Using K-Means Clustering

## Project Overview
This project focuses on segmenting an e-commerce company's customers based on their purchasing behaviour using RFM Analysis and the K-Means Clustering algorithm.

The main objective is to identify different customer groups and help businesses develop targeted marketing strategies.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset
**Dataset:** UCI Online Retail Dataset

**Source:** https://archive.ics.uci.edu/dataset/352/online+retail

The dataset contains online retail transaction information, including customer IDs, invoice numbers, invoice dates, quantities, and unit prices.

## Project Workflow

1. Loaded and inspected the dataset.
2. Handled missing values and inconsistent records.
3. Removed cancelled transactions and invalid quantities and prices.
4. Calculated Recency, Frequency, and Monetary (RFM) values.
5. Applied StandardScaler for feature normalization.
6. Used the Elbow Method to select the number of clusters.
7. Applied K-Means clustering with four clusters.
8. Visualized customer groups using scatter plots.
9. Analyzed customer segments and suggested marketing strategies.

## Customer Segments

| Cluster | Customer Type | Customers |
|---|---|---:|
| 0 | Regular Customers | 3,054 |
| 1 | At-Risk Customers | 1,067 |
| 2 | VIP Customers | 13 |
| 3 | Loyal Customers | 204 |

Total customers analyzed: **4,338**

## Key Findings

- Cluster 2 has the highest average customer spending.
- Cluster 0 represents the largest customer segment.
- Cluster 1 contains customers with high recency values, indicating a long gap since their last purchase.
- Cluster 3 represents customers with recent and frequent purchases.

## Marketing Recommendations

- Regular Customers: Provide personalized offers and discounts.
- At-Risk Customers: Use win-back campaigns and special offers.
- VIP Customers: Provide exclusive benefits and loyalty rewards.
- Loyal Customers: Offer membership benefits and personalized promotions.

## Project Structure

```text
DataAnalytics-L1-CustomerSegmentation/
│
├── dataset/
│   └── Online Retail.csv
│
├── notebook/
│   └── Customer_Segmentation.ipynb
│
├── Output/
│   ├── elbow_method.png
│   ├── recency_frequency_clusters.png
│   ├── frequency_monetary_clusters.png
│   └── customer_count_per_cluster.png
│
└── README.md
```

## Conclusion
This project demonstrates how RFM analysis and K-Means clustering can help businesses understand customer purchasing behaviour, identify valuable customers, improve customer retention, and develop effective marketing strategies.

## Author
Oasis Infobyte Data Analytics Internship – Level 1, Task 2