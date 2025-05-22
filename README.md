# Customer-Segmentation-using-K-Modes
Performed customer clustering on categorical business data using K-Modes, optimized cluster count via Elbow Method, and visualized results with UMAP. Delivered actionable marketing strategies and cluster summaries for business decision-making.


A data-driven customer segmentation project for a leading retailer company of casino gaming machines. The goal was to cluster customers based on their business behavior to inform targeted marketing strategies and sales optimization.

---

## Problem Statement

Company wants to target their customers based on purchasing patterns. To achieve this:
- Developed customer clusters using unsupervised learning.
- Provided statistical summaries and strategic recommendations for each cluster.
- Delivered code notebooks, cluster summaries, visualizations, and business insights.

---


---

## Approach Overview

### 1️⃣ Data Audit & EDA
- Assessed missing values and data quality issues.
- Analyzed feature distributions, inconsistencies, and category frequencies.
- Detected high collinearity using Cramér’s V matrix.

### 2️⃣ Feature Selection
- Dropped redundant, non-behavioral columns (e.g. Customer_ID, address fields).
- Merged highly correlated features (`Casino_Size_Segment` & `Market_Potential_Segment`).
- Retained business-impactful features for clustering.

### 3️⃣ Clustering
- Applied **K-Modes clustering** for categorical data.
- Determined optimal `k=7` using the Elbow Method and cluster performance metrics.
- Named clusters based on revenue, profit, churn risk, market potential, etc.

### 4️⃣ Outlier Detection
- **Categorical Combination Frequency Method**: flagged rare combinations.
- **Isolation Forest** (after one-hot encoding): detected multivariate anomalies.
- Visualized results via PCA.

### 5️⃣ Cluster Visualization
- Visualized clusters in 2D space using **t-SNE**, **PCA**, and **UMAP**.
- UMAP provided the cleanest separation.

### 6️⃣ Business Recommendations
- Benefits Bonanza for loyal, stable customers.
- Increased marketing for high-growth segments.
- Churn management for high-risk clusters.

---

##  Key Deliverables
-  **Final Cluster Summary**: size, high churn %, high revenue %, high propensity %, etc.
-  **Business Interpretation for Each Cluster**
-  **Clean Python notebooks (.ipynb)**
-  **Presentation deck (.pptx) summarizing approach, results & strategy**
-  **Data Quality Checks log**

---

## Assumptions
- Business-calculated segments are reliable.
- 'Missing' retained as a category where relevant.
- Categorical-only clustering via K-Modes (no numerical scaling needed).
- 5% contamination assumption for Isolation Forest.

---

## ⚙Environment & Dependencies

- Python 3.10+
- pandas
- numpy
- scikit-learn
- kmodes
- seaborn
- matplotlib
- umap-learn
