# E-commerce-User-Behavior-Segmentation
E-commerce Customer Segmentation with Hierarchical Clustering
This repository contains a data science project that demonstrates the use of unsupervised machine learning to perform customer segmentation for an e-commerce business. The project uses the Online Retail Dataset (UCI) to identify distinct customer groups based on their purchasing behavior.

Table of Contents
1.Project Overview

2.Methodology

3.Dataset

4.Key Insights

5.Code Structure

Technologies Used

Project Overview
The primary goal of this project is to apply Hierarchical Clustering, a type of unsupervised machine learning, to a transactional dataset. By doing so, we aim to uncover natural groupings of customers and create meaningful segments. The insights gained from these segments can be used to inform targeted marketing strategies, improve customer retention, and increase profitability.

Methodology
The project follows a structured three-phase approach:

Data Preparation: The raw transactional data is preprocessed and cleaned. The core of this step involves RFM (Recency, Frequency, Monetary) analysis to transform the raw data into three key features for each customer:

Recency: Days since the last purchase.

Frequency: Total number of unique purchases.

Monetary: Total money spent.

Model Application: The AgglomerativeClustering algorithm from scikit-learn is applied to the scaled RFM data. A dendrogram is used to visually determine the optimal number of clusters before running the model.

Analysis & Visualization: The final clusters are analyzed by calculating their average RFM scores to understand the profile of each segment. The results are visualized using 2D pair plots and a 3D scatter plot to showcase the cluster separation.

Dataset
The project uses the Online Retail Dataset from the UCI Machine Learning Repository. This is a transactional dataset containing all the purchases made by a UK-based online retailer over a two-year period.

Key Insights
The clustering process revealed three distinct customer segments:

High-Value Champions: These customers have low Recency, high Frequency, and high Monetary values. They are your most loyal and profitable segment.

At-Risk Customers: Characterized by high Recency, low Frequency, and low Monetary values. These customers are at risk of churning and require re-engagement.

New/Emerging Customers: This group has low Recency but low-to-moderate Frequency and Monetary values, indicating they are new and have the potential to become loyal customers.

Code Structure
The main script for this project is customer_segmentation.py. It is a self-contained Python script that performs all the necessary steps from data loading to visualization and analysis.

Technologies Used
Python

Pandas

Scikit-learn

Matplotlib

Seaborn
