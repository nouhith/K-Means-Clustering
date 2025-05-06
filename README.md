# 🛍️ Mall Customer Segmentation using K-Means Clustering

This project applies **unsupervised learning** techniques—specifically **K-Means Clustering**—to segment customers in a mall based on their spending behavior. By analyzing the `Mall_Customers.csv` dataset, the project aims to identify distinct groups of shoppers for targeted marketing strategies.

The notebook also includes **PCA (Principal Component Analysis)** for dimensionality reduction, **Elbow Method** and **Silhouette Score** to determine the optimal number of clusters.

---

## 📁 File Structure

- `K_means_Clustering.ipynb`  
  ➤ Main notebook that contains all the preprocessing, clustering, and visualization steps.

- `data/Mall_Customers.csv`  
  ➤ Dataset containing customer demographic and behavioral features.

---

## 🎯 Objective

The primary objective is to perform **customer segmentation** using unsupervised clustering techniques, helping businesses better understand and target different customer groups based on:

- Age  
- Annual Income (k$)  
- Spending Score (1–100)  

---

## 📊 Data Overview

The dataset includes the following features:

- **CustomerID** — Unique identifier
- **Gender** — Male or Female
- **Age** — Customer age
- **Annual Income (k$)** — Annual income in thousands
- **Spending Score (1–100)** — Score assigned by the mall based on spending behavior

---

## 🧠 Workflow Summary

### 1. 📌 Data Preprocessing

- Load dataset using `pandas`
- Remove unnecessary columns (`CustomerID`)
- Handle categorical encoding (if using `Gender`)
- Normalize features with `StandardScaler`

---

### 2. 📉 Dimensionality Reduction (PCA)

- Applied **Principal Component Analysis** to reduce multi-dimensional data to 2 components for visualization
- PCA helps uncover latent structures in the data and facilitates cleaner cluster plots

---

### 3. 📍 Optimal Cluster Determination

#### 🦴 Elbow Method

- Plots **Within-Cluster Sum of Squares (WCSS)** for different values of `k`
- Optimal `k` chosen at the "elbow" point where WCSS starts diminishing

#### 📈 Silhouette Score

- Evaluates how similar each data point is to its own cluster vs. other clusters
- Higher silhouette score implies better-defined clusters

---

### 4. 🤖 K-Means Clustering

- Clustering applied using `sklearn.cluster.KMeans`
- Final number of clusters based on Elbow + Silhouette analysis
- Centroids computed and plotted

---

### 5. 🧾 Visualizations

- **Elbow Curve** to determine optimal `k`
- **Silhouette Scores** for different values of `k`
- **2D Cluster Plot** after PCA projection
- **Final segmented customer groups** visualized with colors and centroids

---

## 🔧 Tools & Libraries Used

- **Python 3.x**
- **Pandas** – Data loading and manipulation
- **NumPy** – Mathematical operations
- **Matplotlib** & **Seaborn** – Visualization
- **Scikit-learn** – PCA, KMeans, Silhouette Score, StandardScaler

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/mall-customer-segmentation.git
cd mall-customer-segmentation
````

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Run the Notebook

```bash
jupyter notebook K_means_Clustering.ipynb
```

---

## 💡 Key Takeaways

* Applied **unsupervised learning** to perform meaningful customer segmentation
* Used **PCA** to reduce dimensions and improve interpretability
* Determined optimal cluster count using **Elbow Method** and **Silhouette Score**
* Visualized distinct customer segments for business insights

---

## 👨‍💻 Author

Created by **Nouhith**
Feel free to explore, fork, and contribute to the project!

---

