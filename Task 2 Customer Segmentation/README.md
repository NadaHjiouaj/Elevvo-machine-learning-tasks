# Customer Segmentation Analysis

## 📊 Project Overview
This project performs customer segmentation using unsupervised machine learning techniques on the Mall Customers dataset. The goal is to group customers based on their annual income and spending score to identify distinct customer segments for targeted marketing strategies.

## 📁 Dataset
- **Source**: [Mall Customers Dataset on Kaggle](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Features**:
  - CustomerID
  - Gender
  - Age
  - Annual Income (k$)
  - Spending Score (1-100)

## 🎯 Objectives
1. Perform exploratory data analysis and visualize distributions
2. Apply feature scaling
3. Use K-Means clustering to segment customers
4. Determine optimal number of clusters using elbow method and silhouette score
5. Visualize clusters in 2D space
6. (Bonus) Compare with other clustering algorithms (DBSCAN, Agglomerative Clustering)
7. Analyze average spending per cluster

## 🛠️ Tools & Technologies
- **Python**
- **Pandas** - Data manipulation and analysis
- **Matplotlib/Seaborn** - Data visualization
- **Scikit-learn** - Machine learning algorithms
  - StandardScaler - Feature scaling
  - KMeans, DBSCAN, AgglomerativeClustering - Clustering algorithms
  - silhouette_score - Cluster evaluation

## 📈 Key Steps
1. Data loading and initial exploration
2. Visualization of feature distributions
3. Data preprocessing and scaling
4. Determining optimal cluster count
5. Applying K-Means clustering
6. Cluster visualization and analysis
7. (Bonus) Experimenting with alternative clustering approaches

## 📋 Results
The analysis identifies X distinct customer segments based on income and spending patterns. Each cluster represents a different customer profile that can be targeted with specific marketing strategies.

## 🚀 How to Run
1. Install required libraries: `pip install numpy pandas matplotlib seaborn scikit-learn`
2. Run the Jupyter notebook `Customer_Segmentation.ipynb`
3. The dataset will be automatically downloaded from the provided URL

## 📊 Sample Visualizations
- Distribution plots for age, income, and spending score
- Scatter plots showing cluster formations
- Elbow method plot for optimal K determination
- Silhouette score analysis
