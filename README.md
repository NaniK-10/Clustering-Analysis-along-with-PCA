# Clustering Analysis using DBSCAN, PCA and K-Means

This project explores unsupervised clustering techniques on synthetic datasets using density-based and centroid-based algorithms.

The objective is to analyze how clustering algorithms behave on datasets with different shapes and structures.

---

## Overview

Clustering is a fundamental task in unsupervised machine learning used to discover hidden patterns in data without labeled outputs.

In this project, multiple clustering techniques were applied and compared on different datasets to understand their strengths and limitations.

---

## Datasets Used

Three synthetic datasets were used for experimentation:

• **Blob dataset** – compact spherical clusters  
• **Moon dataset** – non-linear moon-shaped clusters  
• **Circle dataset** – concentric circular clusters  

These datasets allow testing how clustering algorithms perform on **different cluster geometries**.

---

## Project Workflow

### 1. Data Exploration
- Loaded datasets using **Pandas**
- Inspected dataset structure and distribution
- Visualized cluster shapes

---

### 2. DBSCAN Clustering

DBSCAN (Density Based Spatial Clustering of Applications with Noise) was applied to identify clusters based on density.

Key concepts used:

- **eps (ε)** – neighborhood radius
- **min_samples** – minimum points required to form a cluster

Clusters and noise points were detected automatically.

---

### 3. K-Distance Graph Analysis

To determine a suitable **ε value**, a **k-distance graph** was plotted.

This helps identify the point where distances sharply increase, indicating the optimal epsilon threshold.

---

### 4. Dimensionality Reduction using PCA

Principal Component Analysis (PCA) was applied to:

- reduce data dimensionality
- analyze clustering behavior in **1D space**

Clustering was then re-performed on the PCA-transformed data.

---

### 5. DBSCAN on Reduced Data

After PCA transformation:

- clustering was performed again in **1D**
- results were compared with original clustering results

---

### 6. K-Means Comparison

To compare clustering approaches:

- **K-Means clustering** was applied
- performance compared against DBSCAN

Key observation:

K-Means struggles with **non-linear cluster shapes**, while DBSCAN can detect arbitrarily shaped clusters.

---

## Key Observations

• DBSCAN performs well on **non-linear cluster structures**  
• K-Means works best for **spherical clusters**  
• PCA dimensionality reduction changes cluster separability  
• Selecting the right **ε value** is crucial for DBSCAN performance  

---

## Technologies Used

Python  
NumPy  
Pandas  
Matplotlib  
Seaborn  
Scikit-learn  
Jupyter Notebook

---

## Repository Structure

```
clustering-analysis
│
├── clustering_analysis.ipynb
└── README.md
```

---

## Future Improvements

Possible extensions for this project:

- Use **hierarchical clustering**
- Apply **OPTICS clustering**
- Perform clustering on **real-world datasets**
- Evaluate clusters using **silhouette score**

---

## Author

Karanam Purna Charan  
B.Tech – Artificial Intelligence & Data Science  
IIT Patna  

GitHub: https://github.com/NaniK-10  
LinkedIn: https://www.linkedin.com/in/purna-charan-karanam-a71477327/
