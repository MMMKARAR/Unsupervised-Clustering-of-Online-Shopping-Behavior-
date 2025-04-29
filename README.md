# 🛍️ Unsupervised Clustering of Online Shopping Behavior

This project explores unsupervised learning techniques to identify behavioral patterns in e-commerce website user sessions. It uses clustering to segment users without relying on purchase labels (Revenue), helping businesses tailor their strategies through data-driven insights.

---

## 📁 Dataset

- **Source**: [UCI Online Shoppers Intention Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail), https://github.com/MMMKARAR/Unsupervised-Clustering-of-Online-Shopping-Behavior-/blob/main/online_shoppers_intention%20Revenue%20removed.csv
- **Modifications**: Revenue column has been removed to enforce a purely unsupervised approach.

---

## 📊 Key Features

- **Numerical**: `Administrative_Duration`, `Informational_Duration`, `ProductRelated_Duration`, `BounceRates`, `ExitRates`, `PageValues`, `SpecialDay`
- **Categorical**: `Month`, `VisitorType`, `Weekend`

---

## 🧪 Workflow Summary

1. **Exploratory Data Analysis**  
   - Visualized distributions for categorical and numerical features.

2. **Preprocessing**  
   - One-hot encoding of categorical features  
   - Scaling of numerical features using `StandardScaler`

3. **Clustering Techniques**  
   - **K-Means** with elbow method to identify optimal clusters  
   - **UMAP + DBSCAN** for non-linear structure discovery

4. **Visualization**  
   - PCA and UMAP projections to view cluster separation

5. **Interpretation**  
   - Behavioral profiling of each cluster  
   - Boxplots and summary statistics

6. **Evaluation**  
   - Silhouette score for K-Means cluster quality

---

## 📈 Tools & Libraries Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn
- UMAP
- DBSCAN
- Imbalanced-learn (for future extension)
- Jupyter Notebook

---

## 🧠 Insights & Use Cases

- **Cluster 0**: Engaged users → Loyalty program targets  
- **Cluster 1**: High exit rates → Use live chat or exit-intent prompts  
- **Cluster 2**: High value seekers → Personalized offers

