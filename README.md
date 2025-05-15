# Unsupervised-learning
Unsupervised Machine Learning projects focused on clustering, dimensionality reduction, and association rule mining with real-world datasets

 # 🛍 Customer Segmentation Using Association Rule Mining, Clustering, and Dimensionality Reduction

## 📊 Project Overview

This project delves into the Online Retail II dataset to perform customer segmentation using a combination of: 

Association Rule Mining: Uncovering relationships between products purchased together.

RFM Analysis: Evaluating customer behavior based on Recency, Frequency, and Monetary metrics.

Clustering (KMeans): Grouping customers into distinct segments based on RFM features.

Dimensionality Reduction (PCA & t-SNE): Visualizing high-dimensional data in two dimensions for better interpretability.

The goal is to provide actionable insights into customer purchasing patterns, enabling businesses to tailor marketing strategies effectively. 

## 📁 Dataset

### Source: UCI Machine Learning Repository

### Description:
Transactions from a UK-based online retailer between 2009 and 2011, primarily selling unique giftware.

### Attributes:

InvoiceNo: Unique invoice number.

StockCode: Product (item) code.

Description: Product name.

Quantity: Number of products per transaction.

InvoiceDate: Date and time of the transaction.

Price: Unit price of the product.

Customer ID: Unique identifier for each customer.

Country: Country of the customer. 

## 🧰 Methodology

### 1. Data Preprocessing

Removed entries with missing Customer ID.

Excluded canceled transactions (identified by invoices starting with 'C').

Filtered out records with non-positive Quantity or Price.

Created a new feature TotalPrice as Quantity * Price. 


### 2. Association Rule Mining

Utilized the Apriori algorithm to identify frequent itemsets.

Generated association rules to discover product combinations frequently bought together.

Visualized top rules using network graphs to depict product relationships. 

### 3. RFM Analysis

Recency: Days since the customer's last purchase.

Frequency: Total number of purchases made by the customer.

Monetary: Total amount spent by the customer.

Standardized RFM features for uniform scaling. 


### 4. Clustering

Applied KMeans clustering to segment customers based on RFM scores.

Determined the optimal number of clusters using the Elbow Method.

Analyzed cluster characteristics to profile customer segments. 


### 5. Dimensionality Reduction

PCA (Principal Component Analysis):

Reduced RFM features to two principal components.

Visualized customer clusters in a 2D space.

t-SNE (t-distributed Stochastic Neighbor Embedding):

Further visualized high-dimensional data in two dimensions.

Enhanced the interpretability of customer segments. 

## 📌 Results

Identified key product associations, aiding in cross-selling strategies.

Segmented customers into distinct groups:

High-Value Customers:  Frequent purchasers with high spending.

At-Risk Customers: Long time since last purchase.

New Customers: Recent purchasers with limited transaction history.

Visualizations provided clear insights into customer behaviors and preferences. 

## 🛠 Requirements

Ensure the following Python libraries are installed:

pip install pandas numpy matplotlib seaborn scikit-learn mlxtend networkx openpyxl

### 🚀 Getting Started

#### 1. Download the Dataset:

Obtain the Online Retail II dataset from 
https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci?select=online_retail_II.csv


#### 2. Run the Analysis:

Open the customer_segmentation.ipynb notebook.
Execute cells sequentially to perform data preprocessing, analysis, and visualization. 


## 📈 Visualizations

Association Rules Network :- Graph depicting relationships between frequently purchased products.

RFM Distribution :- Histograms showcasing the distribution of Recency, Frequency, and Monetary scores.

PCA Plot :- 2D scatter plot illustrating customer clusters based on principal components.

t-SNE Plot :- Enhanced visualization of customer segments in two dimensions. 

## 📚 References

Online Retail II Dataset - https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci?select=online_retail_II.csv

Apriori Algorithm - mlxtend Documentation

KMeans Clustering - scikit-learn Documentation

PCA - scikit-learn Documentation

t-SNE - scikit-learn Documentatio

## Contact Information

📌 Name : Bhumika Kadbe

📌 Email: bhumikakadbe@gmail.com

📌 LinkedIn:(https://www.linkedin.com/in/bhumika-kadbe-20409331b?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BhhLvRrNXRk%2B3zu%2BT3UDxkg%3D%3D)

💬 Feel free to reach out for collaborations, discussions, or queries related to this project.












