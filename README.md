# E-commerce-User-Behavior-Segmentation
****E-commerce Customer Segmentation with Hierarchical Clustering***
This repository documents a data science project on the application of unsupervised machine learning to segment the customer base of an e-commerce enterprise. The project utilizes the Online Retail Dataset (UCI) to identify distinct customer groups based on their purchasing behavior.

* Table of Contents
1 Project Overview

2 Methodology

3 Dataset

4 Key Insights

5 Code Structure

6 Technologies Used

1.Project Overview:
The primary objective of this project is to apply Hierarchical Clustering to a transactional dataset. This initiative seeks to identify inherent customer groupings and develop meaningful segments. The derived insights are instrumental in informing targeted marketing strategies, enhancing customer retention, and bolstering overall profitability.

2.Methodology:
The project employs a structured three-phase approach:

i.Data Preparation: This phase involves the preprocessing and cleaning of raw transactional data. A central component is RFM (Recency, Frequency, Monetary) analysis, which transforms the raw data into three key customer features:

*Recency: The duration in days since a customer's last purchase.

*Frequency: The total count of unique purchases.

*Monetary: The cumulative monetary value of all purchases.

ii.Model Application: The AgglomerativeClustering algorithm from scikit-learn is applied to the scaled RFM data. A dendrogram is utilized to visually inform the selection of an optimal number of clusters prior to model execution.

iii.Analysis & Visualization: The final clusters are profiled by computing their average RFM metrics to ascertain the characteristics of each segment. The results are then visualized using 2D pair plots and a 3D scatter plot to illustrate the distinct separation of the clusters.

3.Dataset:
This project utilizes the Online Retail Dataset from the UCI Machine Learning Repository, a transactional record of purchases from a UK-based online retailer over a two-year period.

4.Key Insights:
The clustering process revealed three distinct customer segments:

High-Value Champions: This segment exhibits low Recency, high Frequency, and high Monetary values, suggesting a profile of highly loyal and profitable customers.

At-Risk Customers: Characterized by high Recency, low Frequency, and low Monetary values, this group consists of customers who may be considered at risk of attrition.

New/Emerging Customers: This cluster is distinguished by low Recency in conjunction with low-to-moderate Frequency and Monetary values, which may indicate a newly acquired customer base with the potential for future loyalty.

5.Code Structure:
The core of this project is a self-contained Python script, customer_segmentation.py, which performs all requisite steps from data acquisition to visualization and analysis.

6.Technologies Used:
*Python

*Pandas

*Scikit-learn

*Matplotlib

*Seaborn
