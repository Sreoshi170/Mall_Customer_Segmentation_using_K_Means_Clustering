# 🛍️ Mall Customer Segmentation using K-Means Clustering

This project applies **K-Means Clustering** to segment customers based on their age, annual income, and spending score. Using **unsupervised learning**, we identify meaningful customer groups to help businesses target different market segments more effectively.

---

## 📊 Dataset Overview

* **Dataset:** `Mall_Customers.csv`
* **Total Customers:** 200
* **Features Used:**

  * Gender (encoded)
  * Age
  * Annual Income (k\$)
  * Spending Score (1–100)

---

## ✅ Project Workflow

### 1. Data Preprocessing

* Dropped `CustomerID` as it's non-informative
* Converted `Gender` to numeric via one-hot encoding
* Scaled features using `StandardScaler`

### 2. Dimensionality Reduction

* Applied **PCA** to reduce the feature space to 2 dimensions
* Visualized customer distribution by gender

### 3. K-Means Clustering

* Assumed `K=5` initially and trained a **KMeans** model
* Visualized clusters using the PCA-reduced 2D space

### 4. Elbow Method

* Used **within-cluster sum of squares (inertia)** to identify the optimal number of clusters
* Elbow appeared around **K=5**, supporting initial assumption

### 5. Cluster Evaluation

* Calculated the **Silhouette Score** to assess clustering quality
* Higher score confirmed well-separated, compact clusters

---

## 📈 Visualizations

* 🎨 PCA scatter plot with gender-based coloring
* 📍 K-Means cluster visualization in 2D
* 🔍 Elbow curve to determine optimal `K`
* 🌀 Cluster visualization with color-coded segments

---

## 🧠 Techniques Used

* K-Means Clustering
* Principal Component Analysis (PCA)
* Silhouette Score for evaluation
* Elbow Method for optimal K estimation
* Feature Standardization
* One-Hot Encoding

---

## 🧰 Tools & Libraries

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 🔗 Notebook Access

View the full notebook here:
👉 [Open in Colab](https://colab.research.google.com/drive/1mYKy6R_mDgzqa8Q2q8IqvcuA8z3TweoN)

