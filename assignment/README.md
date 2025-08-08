# 📚 HOMEWORK ASSIGNMENT - Hierarchical Clustering

## 📌 Overview

This project demonstrates how to perform **Hierarchical Clustering** on the Wholesale Customers Dataset.  
Hierarchical clustering is an **unsupervised machine learning** technique used to group similar data points into clusters, without requiring predefined labels.  
It builds a hierarchy of clusters that can be visualized using a **dendrogram**.

## 📂 Dataset

The dataset contains annual spending amounts for customers of a wholesale distributor, along with categorical indicators for their **business type** and **geographical region**.

### Columns

| Column               | Description                                                              |
| -------------------- | ------------------------------------------------------------------------ |
| **Channel**          | Type of customer: `1` = Horeca (Hotel/Restaurant/Café), `2` = Retail     |
| **Region**           | Geographical region: `1` = Lisbon, `2` = Oporto, `3` = Other             |
| **Fresh**            | Annual spending on fresh products (fruits, vegetables, meat, fish, etc.) |
| **Milk**             | Annual spending on milk and milk-based products                          |
| **Grocery**          | Annual spending on grocery items (non-perishable food, dry goods, etc.)  |
| **Frozen**           | Annual spending on frozen products                                       |
| **Detergents_Paper** | Annual spending on detergents and paper products                         |
| **Delicatessen**     | Annual spending on delicatessen (gourmet foods, specialty items)         |

## 🎯 Objective

- **Preprocess** the dataset (handle scaling and normalization)
- **Apply Hierarchical Clustering** to group customers based on their purchasing patterns
- **Visualize** the clusters using a dendrogram and scatter plots
- Interpret the clusters in the context of customer segmentation

## 🛠️ Methodology

1. **Data Preprocessing**
   - Removed non-numeric identifiers if needed
   - Scaled features to normalize different spending ranges
2. **Model Building**
   - Used `scipy.cluster.hierarchy` to perform Agglomerative Hierarchical Clustering
   - Tried different linkage methods: `"ward"`, `"complete"`, `"average"`
3. **Cluster Selection**
   - Used a dendrogram to decide the optimal number of clusters
4. **Visualization**
   - Plotted dendrogram to show cluster hierarchy
   - Reduced dimensions using PCA for cluster visualization in 2D
