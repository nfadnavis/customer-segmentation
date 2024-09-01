# customer-segmentation
Customer Segmentation Using Online Retail Data
Overview
This project focuses on customer segmentation using transactional data from an online retail store. The goal is to categorize customers into distinct segments based on their purchasing behavior using Recency, Frequency, and Monetary (RFM) analysis, followed by K-Means clustering. Additionally, a Random Forest classifier is used to evaluate the model’s ability to predict customer segments.

Table of Contents
Overview
Data
Project Steps
Results
How to Run
Dependencies
License
Data
The dataset used in this project is from the UCI Machine Learning Repository. It consists of transactional data from a UK-based online retail store between 2010 and 2011. Key features include:

InvoiceNo: Unique identifier for each transaction.
StockCode: Unique product identifier.
Description: Product description.
Quantity: The quantity of each product per transaction.
InvoiceDate: The date and time of the transaction.
UnitPrice: Price per unit of product.
CustomerID: Unique identifier for each customer.
Country: Country of the customer.
Project Steps
Data Preprocessing:

Convert InvoiceDate to datetime format.
Filter out canceled transactions.
Calculate Recency, Frequency, and Monetary values for each customer.
RFM Analysis:

Generate an RFM table summarizing key metrics.
Use the Elbow Method to determine the optimal number of clusters.
Apply K-Means clustering to segment customers.
Clustering Evaluation:

Evaluate the quality of clustering using the Silhouette Score.
Visualize customer segments through scatter plots.
Cluster Analysis:

Analyze characteristics of each cluster.
Highlight key insights from the clusters.
Random Forest Classifier:

Build and train a Random Forest model to classify customers into clusters.
Evaluate the classifier's performance using accuracy, precision, recall, and F1-score.
Visualize feature importance and the structure of a decision tree from the Random Forest model.
Results
RFM Table Summary
The RFM table provides insights into how different customer segments are distributed based on their purchasing behavior. Key metrics like Recency, Frequency, and Monetary values are color-coded for easy interpretation.

Clustering Results
The Elbow Method suggests using 4 clusters, which were validated by the Silhouette Score. The clustering visualizations show distinct segments of customers based on Recency vs. Frequency, Monetary vs. Frequency, and Recency vs. Monetary.

Random Forest Classifier
The Random Forest classifier achieved high accuracy, precision, recall, and F1-score, indicating that the model effectively predicts customer segments. Feature importance analysis shows the impact of Recency, Frequency, and Monetary values on the classification.
