## Customer Segmentation and Coupon Usage Analysis

# Overview
This project analyzes customer behavior based on transaction data and coupon usage to identify distinct customer segments. The goal is to provide targeted recommendations for enhancing customer engagement and loyalty through effective marketing strategies.

# Dataset
The dataset contains the following features:
* Transaction Count: The number of transactions made by the customer.
* Coupon Usage: The number of coupons used by the customer.
* Days Since Last Transaction: The number of days since the customer's last transaction.

# Approach

* **1.Data Import and Cleaning**
  * Data Import: Load the dataset containing customer transaction and coupon usage data.
  * Data Cleaning: Address missing values, remove duplicates, and handle any inconsistencies in the data.
* **2.Exploratory Data Analysis (EDA)**
  * Data Exploration: Analyze the distribution and summary statistics of the features.
  * Visualization: Create visualizations to understand relationships between variables and identify patterns.
  * Correlation Analysis: Investigate correlations between features and the target variable.
* **3.Data Preprocessing**
  * Cleaned the dataset by handling missing values and outliers.
  * Encoded categorical variables and normalized numerical features.
* **4.Feature Selection**
   Identified and selected relevant features that contribute to the prediction of customer behavior.
* **5.Model Training and Evaluation**
  * Applied various machine learning models, including:
    * *K-means*: A partitioning method that clusters data into K distinct groups based on feature similarity.
    * *Hierarchical Clustering*: A method that builds a hierarchy of clusters, allowing for the visualization of data at multiple levels of granularity.
    * *DBSCAN*: A density-based clustering algorithm that identifies clusters based on the density of data points, useful for detecting noise and outliers.
   
  * Model Evaluation: Used metrics such as inertia and silhouette score to assess clustering performance and determine the optimal number of clusters.

# Customer Behavior Summary:
* **Cluster 0**
  * Average Transaction Count: 7.685398230088496
  * Average Coupon Usage: 4.280973451327434
  * Average Days Since Last Transaction: 281.98362831858407
* **Cluster 1**
  * Average Transaction Count: 5.032228360957642
  * Average Coupon Usage: 2.3213627992633517
  * Average Days Since Last Transaction: 655.1629834254144
* **Cluster 2**
  * Average Transaction Count: 4.357607282184655
  * Average Coupon Usage: 1.6781534460338101
  * Average Days Since Last Transaction: 197.32119635890768

# Recommendations
* **Cluster 0**
  * High-frequency, high-transaction customers with frequent coupon usage.
  * Offer loyalty discounts or exclusive high-value coupons.
* **Cluster 1**
  * Low-frequency customers with smaller transactions and moderate coupon usage.
  * Provide time-limited offers or discounts to encourage more frequent transactions.
* **Cluster 2**
  * Customers with fewer coupon usages and irregular shopping patterns.
  * Provide introductory or higher-value coupons to incentivize coupon usage and increase engagement.
