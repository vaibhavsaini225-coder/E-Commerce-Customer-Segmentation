# 🛒 E-Commerce Customer Segmentation Using Machine Learning

## 📌 Project Overview

This project focuses on segmenting e-commerce customers based on their purchasing behavior using **K-Means and DBSCAN clustering algorithms**.

The project uses the RFM (Recency, Frequency, Monetary) model to understand customer behavior, applies PCA for dimensionality reduction, and uses t-SNE to visualize customer segments. Finally, actionable marketing personas are derived to help businesses improve customer retention, engagement, and sales.

## 🎯 Objectives

* Analyze customer purchasing behavior using RFM analysis.
* Segment customers using K-Means clustering.
* Identify customer groups and potential outliers using DBSCAN.
* Apply Principal Component Analysis (PCA) for dimensionality reduction.
* Visualize customer segments using t-SNE.
* Evaluate clustering performance using the Silhouette Score.
* Develop actionable marketing personas for different customer segments.

## 📊 Dataset

**Dataset Name:** Online Retail Dataset

**Source:** UCI Machine Learning Repository

**Download Dataset:** https://archive.ics.uci.edu/static/public/352/online+retail.zip

The dataset contains transactions from a UK-based online retailer between December 2010 and December 2011.

It includes approximately 541,909 transaction records.

### Dataset Features

| Feature     | Description                              |
| ----------- | ---------------------------------------- |
| InvoiceNo   | Unique transaction or invoice identifier |
| StockCode   | Unique product identifier                |
| Description | Product description                      |
| Quantity    | Number of items purchased                |
| InvoiceDate | Date and time of the transaction         |
| UnitPrice   | Price per item                           |
| CustomerID  | Unique customer identifier               |
| Country     | Customer's country                       |

**Note:** The dataset contains missing customer IDs, cancelled transactions, and returns. These are handled during preprocessing.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab
* Jupyter Notebook

## 🧠 Methodology

### 1. Data Collection

Download the Online Retail dataset from the UCI Machine Learning Repository.

### 2. Data Preprocessing

* Handle missing customer IDs.
* Remove cancelled transactions.
* Filter invalid quantities and prices.
* Convert transaction dates into datetime format.
* Calculate the total transaction amount.

### 3. RFM Analysis

Three customer-level features are calculated:

* **Recency:** Number of days since the customer's most recent purchase. Lower values indicate more recent activity.
* **Frequency:** Number of distinct invoices associated with the customer.
* **Monetary:** Total amount spent by the customer.

### 4. Feature Transformation and Scaling

Apply logarithmic transformation to reduce skewness and use RobustScaler to scale RFM features.

### 5. K-Means Clustering

Use the Elbow Method to help select the number of clusters and segment customers according to their RFM characteristics.

### 6. DBSCAN Clustering

Apply density-based clustering to identify customer groups and detect potential noise points or outliers.

### 7. Dimensionality Reduction Using PCA

Reduce the three RFM features to two principal components for visualization.

### 8. Customer Visualization Using t-SNE

Project customer data into two dimensions to visualize local patterns and relationships between customer segments.

### 9. Model Evaluation

Evaluate the clustering results using the Silhouette Score, cluster sizes, and RFM profiles.

### 10. Marketing Persona Development

Interpret customer segments and recommend targeted marketing strategies.

## 📈 Expected Marketing Personas

The actual personas depend on the clusters discovered in the dataset.

| Customer Persona | Characteristics                                  | Marketing Strategy               |
| ---------------- | ------------------------------------------------ | -------------------------------- |
| Champions        | Recent purchases, frequent orders, high spending | VIP rewards and exclusive offers |
| Loyal Customers  | Frequent and relative                            |                                  |
