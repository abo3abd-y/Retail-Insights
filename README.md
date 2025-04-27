# Retail-Insights

# 🛒 Customer Purchase Behavior Analysis

## Overview

This project analyzes customer transaction data from an e-commerce platform to uncover hidden patterns in purchasing behavior and segment customers based on their shopping habits. By leveraging data mining and clustering techniques, we aim to extract actionable insights that can enhance product recommendations, personalized marketing, and customer retention strategies.

---

## Objective

- **Identify frequently co-purchased items** using **Frequent Itemset Mining** with the **Apriori Algorithm**.
- **Segment customers into meaningful groups** based on their shopping behavior using:
  - **K-Means Clustering**
  - **Gaussian Mixture Models (GMM)**
- **Visualize** the findings to better understand purchase relationships and customer segmentation.

---

## Dataset

- **Source:** [Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail) from the UCI Machine Learning Repository.
- **Description:**  
  Transactional data for a UK-based online retailer.  
  Fields include:
  - `InvoiceNo`
  - `StockCode`
  - `Description`
  - `Quantity`
  - `InvoiceDate`
  - `UnitPrice`
  - `CustomerID`
  - `Country`

---

## Methods and Techniques

- **Data Preprocessing:**
  - Removal of missing values.
  - Exclusion of canceled transactions.
  - Filtering invalid (negative) quantities and prices.

- **Frequent Itemset Mining:**
  - Applied the **Apriori Algorithm** to identify common sets of products purchased together.
  - Generated **Association Rules** to find strong relationships between products.

- **Customer Segmentation:**
  - Performed **RFM Analysis** (Recency, Frequency, Monetary value) to build customer profiles.
  - Scaled features using **StandardScaler** for clustering.
  - Applied **K-Means Clustering** to group customers into discrete segments.
  - Applied **Gaussian Mixture Models (GMM)** to perform soft (probabilistic) clustering.
  - Visualized customer segments using **Principal Component Analysis (PCA)** for 2D representation.

---

## Key Concepts

- **Recency:** How recently a customer made a purchase.
- **Frequency:** How often a customer makes a purchase.
- **Monetary:** How much money a customer spends.

- **Apriori Algorithm:**  
  A popular algorithm for mining frequent itemsets and discovering association rules between items.

- **K-Means Clustering:**  
  A partitioning method that divides data into `k` clusters based on feature similarity.

- **Gaussian Mixture Models (GMM):**  
  A soft clustering approach that models data as a mixture of multiple Gaussian distributions.

- **Principal Component Analysis (PCA):**  
  Dimensionality reduction technique used to project high-dimensional data into 2D for visualization.

---

## Results Summary

- **Frequent Itemsets:**
  - Discovered common combinations of products purchased together (e.g., different styles of lunch bags, tea sets, and home decorations).
  - Identified opportunities for cross-selling and bundling products.

- **Customer Segments:**
  - Segmented customers into distinct groups:
    - **Super Buyers:** Frequent and high-spending customers.
    - **Active Regulars:** Consistent customers with moderate spending.
    - **At-Risk Customers:** Customers with low recency and low spend who may require reactivation.

- **Business Insights:**
  - Suggest bundling strategies based on frequent itemsets.
  - Implement targeted loyalty programs for high-value customer segments.
  - Launch reactivation campaigns for at-risk customers.

---

## Visualizations

- **Top Frequent Itemsets** (bar plots)
- **Association Rule Metrics** (support vs confidence scatter plots)
- **Customer Segmentation** (2D PCA cluster plots for both KMeans and GMM)

---

## Project Structure

