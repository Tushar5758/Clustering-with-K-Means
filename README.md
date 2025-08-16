# K-Means Clustering – Customer Segmentation

## Objective  
The goal of this task is to apply **K-Means clustering** on customer demographic and spending data to identify meaningful customer segments for business insights.

---

## Tools & Libraries  
- Python 3.x  
- Pandas – dataset handling  
- NumPy – numerical operations  
- Matplotlib & Seaborn – visualization  
- Scikit-learn – KMeans, StandardScaler, Silhouette Score, PCA  

---

## Dataset  
The dataset used is the **Mall Customer Segmentation Dataset**, which includes the following features:  

- **CustomerID** – Unique identifier  
- **Gender** – Male/Female (not used directly for clustering)  
- **Age** – Age of the customer  
- **Annual Income (k$)** – Customer income  
- **Spending Score (1-100)** – Spending behavior score  

---

## Steps Implemented  

### 1. Data Preprocessing  
- Selected features: `Age`, `Annual Income (k$)`, `Spending Score (1-100)`  
- Applied **StandardScaler** to normalize data.  

### 2. Elbow Method  
- Computed **WCSS (Within-Cluster Sum of Squares)** for `k = 2 to 10`.  
- Plotted the **Elbow Curve** to find the optimal number of clusters.  

### 3. K-Means Clustering  
- Fitted K-Means with the optimal **k (e.g., 5)**.  
- Assigned cluster labels to each customer.  

### 4. Cluster Evaluation  
- Used **Silhouette Score** to measure cluster quality.  

### 5. Visualization  
- **3D Scatter Plot** of clusters using Age, Income, and Spending Score.  
- **2D PCA Plot** for simplified visualization of clusters.  

### 6. Insights  
- Generated cluster summaries showing **average Age, Income, and Spending Score** for each segment.  
- Example interpretations:  
  - Cluster 0 → Young, high income, high spenders (**premium customers**)  
  - Cluster 1 → Older, moderate income, low spenders (**conservative group**)  
  - Cluster 2 → Young, low income, medium spenders (**budget-conscious**)  
  - Cluster 3 → Middle-aged, high income, low spenders (**potential churn risk**)  
  - Cluster 4 → Middle-aged, high income, high spenders (**VIP segment**)  

---

## Results  

- The **Elbow Method** suggested an optimal `k`.  
- The **Silhouette Score** confirmed clustering quality.  
- Clear segmentation of customer groups was achieved.  

---
