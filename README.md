# 📊 Customer Segmentation using K-Means vs Hierarchical Clustering

## 📌 Overview
This repository contains the implementation and research work from my scientific paper:

"Analisis Komparatif Metode K-Means dan Hierarchical Clustering untuk Segmentasi Pelanggan Pusat Kebugaran"
The study focuses on comparing clustering methods to identify customer segments and support churn reduction strategies in the fitness industry.

## 🎯 Research Objectives
- Compare the performance of K-Means and Hierarchical Clustering
- Identify optimal customer segmentation
- Evaluate clustering quality using multiple metrics
- Provide business insights for customer retention strategy

## 📄 Academic Context
This research was conducted as part of the academic requirement for completing a scientific article in the Statistics program at Universitas Terbuka. This paper has been officially published in:

Prosiding Seminar Nasional Sains dan Teknologi (SAINTEK), Universitas Terbuka

🔗 Full paper:
https://conference.ut.ac.id/index.php/saintek/article/view/7999

## 📊 Dataset
- Source: Kaggle ([Gym Customers Features and Churn](https://www.kaggle.com/datasets/adrianvinueza/gym-customers-features-and-churn))
- Observations: 4000
- Variables: 14 features (demographic & behavioral)

## ⚙️ Methods
Clustering Algorithms:
- K-Means (k-means++)
- Hierarchical Clustering (Ward, Complete, Average)

Evaluation Metrics:
- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Index
- Dunn Index
- Adjusted Rand Index (Stability)
- Execution Time

## 🔄 Research Workflow

The research was conducted through the following structured steps:

### 1. Data Understanding
- Load and explore dataset (4000 observations, 14 variables)
- Identify variable types (categorical & numerical)

### 2. Data Preprocessing
- Missing value & duplicate checking (no issues found)
- Outlier handling using **IQR + Winsorization**
- Multicollinearity analysis (Pearson correlation)
- Feature selection (remove highly correlated variables)
- Standardization using **StandardScaler**

### 3. Determining Optimal Clusters
- Elbow Method (Inertia)
- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Index

→ Optimal number of clusters: **k = 2**

### 4. Model Implementation
#### K-Means
- Initialization: k-means++
- Distance: Euclidean
- Iterative centroid optimization

#### Hierarchical Clustering
- Approach: Agglomerative
- Linkage comparison:
  - Ward
  - Complete
  - Average
- Best linkage: **Complete**

### 5. Model Evaluation
- Silhouette Score (SC)
- Calinski-Harabasz Index (CHI)
- Davies-Bouldin Index (DBI)
- Dunn Index (DI)

### 6. Stability Testing
- Method: Resampling (10 iterations, 80% data)
- Metric: Adjusted Rand Index (ARI)

### 7. Performance Comparison
- Clustering quality
- Stability
- Execution time

### 8. Cluster Interpretation
- Profiling each cluster
- Business interpretation (churn behavior)

### 9. Insight & Recommendation
- Identify high-risk and loyal customers
- Recommend K-Means for real-time segmentation

## 📈 Key Findings
- K-Means outperformed Hierarchical Clustering
- Best number of clusters: k = 2
- Stability (ARI): 0.905
- Execution time: 0.08 seconds

Customer Segments:
#### 1. High-Risk Casual (31.2%)
- Low engagement
- High churn risk (84%)
#### 2. Low-Risk Regular (68.8%)
- Loyal customers
- Very low churn (0.3%)

## 🧠 Business Insight
- High-risk customers require aggressive retention strategies
- Loyal customers should be targeted for long-term value optimization
- K-Means is suitable for real-time segmentation systems

## 🛠️ Tech Stack
- Python 3.12
- Scikit-learn
- SciPy
- Pandas
- Matplotlib / Seaborn / Plotly

## 📂 Repository Structure
- [notebook.ipynb](https://github.com/AdamGustiAndito/Customer-Segmentation-using-K-Means-vs-Hierarchical-Clustering/blob/main/Analisis%20Komparatif%20Metode%20K-Means%20dan%20Hierarchical%20Clustering%20dalam%20Segmentasi%20Pelanggan%20Pusat%20Kebugaran.ipynb) → Full analysis & modeling
- [paper.pdf](https://github.com/AdamGustiAndito/Customer-Segmentation-using-K-Means-vs-Hierarchical-Clustering/blob/main/Analisis%20Komparatif%20Metode%20K-Means%20dan%20Hierarchical%20Clustering%20untuk%20Segmentasi%20Pusat%20Kebugaran.pdf) → Published paper
- [dataset](https://github.com/AdamGustiAndito/Customer-Segmentation-using-K-Means-vs-Hierarchical-Clustering/blob/main/gym_churn_us.csv) → Dataset 

## 👤 Author
Adam Gusti Andito
Statistika - Universitas Terbuka
📧 Contact me:
- [LinkedIn](https://www.linkedin.com/in/adam-gusti-andito-1b04721b0/)
- Email: adam.gustiandito@gmail.com

## ⚠️ License
This project is for academic and research purposes only.
