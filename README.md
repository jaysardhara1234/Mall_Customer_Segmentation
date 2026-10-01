# 🛍️ Mall Customer Segmentation using Clustering

A Machine Learning project that segments mall customers based on their **Annual Income** and **Spending Score** using unsupervised clustering techniques. 🤖📊

## 📌 Project Overview

This project applies and compares three clustering algorithms:

* 🔵 **K-Means Clustering**
* 🌳 **Agglomerative Hierarchical Clustering**
* 🔍 **DBSCAN**

The goal is to identify meaningful **customer segments** that can help with targeted marketing and customer analysis. 🎯

## 📊 Dataset

**Mall Customers Dataset**

The dataset contains customer information such as:

* 👤 Age
* 🚻 Gender
* 💰 Annual Income
* 🛒 Spending Score

For the main clustering analysis, **Annual Income** and **Spending Score** are used to identify distinct customer groups.

## 🔄 Project Workflow

1. 📥 Load and explore the dataset
2. 🧹 Clean and preprocess the data
3. 🔢 Encode categorical features
4. 📏 Scale numerical features using `StandardScaler`
5. 🎯 Select features for clustering
6. 🔵 Apply K-Means
7. 🌳 Apply Agglomerative Clustering
8. 🔍 Apply DBSCAN
9. 📈 Evaluate clusters using Silhouette Score
10. 💡 Analyze customer segments

## 🤖 Clustering Algorithms

### 🔵 K-Means

The **Elbow Method** and **Silhouette Score** are used to determine a suitable number of clusters.

**Number of clusters: 5**

### 🌳 Agglomerative Hierarchical Clustering

A **dendrogram** is used to visualize the hierarchical structure of the customers.

**Number of clusters: 5**

### 🔍 DBSCAN

DBSCAN is tested with different parameter combinations to identify clusters and noise points.

**Selected parameters:**

* `eps = 0.3`
* `min_samples = 5`

## 👥 Customer Segments

The clustering analysis identifies five main customer groups:

| 🏷️ Segment | 📌 Characteristics           |
| ----------- | ---------------------------- |
| 1️⃣         | Medium Income / Medium Spend |
| 2️⃣         | High Income / High Spend     |
| 3️⃣         | Low Income / High Spend      |
| 4️⃣         | High Income / Low Spend      |
| 5️⃣         | Low Income / Low Spend       |

## 📈 Model Evaluation

The clustering models are evaluated using the **Silhouette Score**.

> 💡 A higher Silhouette Score generally indicates better-separated and more compact clusters.

For DBSCAN, noise points (`-1`) are excluded when calculating the Silhouette Score.

The notebook also provides visualizations to compare the clustering results. 📊

## 💡 Business Insights

Customer segmentation can help businesses develop more targeted strategies, such as:

* 🎁 Loyalty rewards for high-value customers
* 🏷️ Personalized offers for medium-spending customers
* 💸 Promotional discounts for price-sensitive customers
* 💎 Premium recommendations for high-income, low-spending customers

## 🛠️ Technologies Used

* 🐍 Python
* 🐼 Pandas
* 🔢 NumPy
* 📊 Matplotlib
* 🎨 Seaborn
* 🤖 Scikit-learn
* 🧮 SciPy
* 📓 Jupyter Notebook

## 📁 Project Structure

```text
📦 Project
├── 📂 Dataset/
│   └── 📄 Mall_Customers.csv
├── 📓 Clustering_Model.ipynb
└── 📖 README.md
```

## 🎯 Project Goal

The main objective of this project is to demonstrate how **unsupervised Machine Learning** can be used to discover customer patterns and create meaningful customer segments from real-world data.

---
