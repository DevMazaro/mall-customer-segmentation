# Mall Customer Segmentation Analysis

A comprehensive customer segmentation analysis using multiple clustering techniques to identify distinct customer groups and provide actionable business insights.

## 📊 Project Overview

This project demonstrates customer segmentation using three different clustering algorithms on mall customer data. The analysis helps businesses understand their customer base and develop targeted marketing strategies.

**Dataset**: Mall Customer Segmentation Data (200 customers)
**Features**: Customer ID, Gender, Age, Annual Income, Spending Score

## 🎯 Business Objectives

- Identify distinct customer segments based on spending behavior and demographics
- Compare effectiveness of different clustering algorithms
- Provide actionable business recommendations for each customer segment
- Optimize marketing strategies and resource allocation

## 🔬 Clustering Methods Used

| Method | Description | Key Strengths |
|--------|-------------|---------------|
| **K-Means** | Partitions data into k clusters using centroids | Fast, scalable, works well with spherical clusters |
| **Hierarchical** | Builds tree-like cluster structure | No need to specify cluster count upfront, shows cluster relationships |
| **DBSCAN** | Density-based clustering that identifies outliers | Finds arbitrary shaped clusters, identifies noise points |

## 📈 Key Findings

### Customer Segments Identified (K-Means Results)

| Segment | Size | Avg Age | Avg Income (\$k) | Avg Spending Score | Profile |
|---------|------|---------|------------------|-------------------|---------|
| **Standard Shoppers** | 81 (40.5%) | 42.7 | 55.3 | 49.5 | Middle-income, moderate spenders |
| **Premium Shoppers** | 39 (19.5%) | 32.7 | 86.5 | 82.1 | High-income, high spenders |
| **Fashion-Forward Youth** | 22 (11%) | 25.3 | 25.7 | 79.4 | Low-income, high spenders |
| **Affluent Conservatives** | 35 (17.5%) | 41.1 | 88.2 | 17.1 | High-income, low spenders |
| **Budget Conservatives** | 23 (11.5%) | 45.2 | 26.3 | 20.9 | Low-income, low spenders |

### Business Insights

- **Premium Shoppers** (19.5% of customers) likely contribute disproportionately to revenue
- **Affluent Conservatives** represent significant untapped potential - high income but low engagement
- **Fashion-Forward Youth** show high loyalty potential as their earning power increases
- **Standard Shoppers** form the backbone of consistent revenue

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-learn** - Machine learning algorithms
- **SciPy** - Scientific computing and hierarchical clustering

## 📋 Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
scipy
```

## 🚀 Getting Started

### Run in Google Colab (Recommended)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DevMazaro/mall-customer-segmentation/blob/main/mall_customer_segmentation.ipynb)

### Local Jupyter Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/DevMazaro/mall-customer-segmentation.git
   cd mall-customer-segmentation

2. Install required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy jupyter
   ```

3. Run the analysis:
   ```bash
   jupyter notebook mall_customer_segmentation.ipynb
   ```

## 📊 Analysis Workflow

1. **Data Exploration** - Statistical analysis and visualization of customer demographics
2. **Feature Selection** - Identifying optimal features for clustering (Income vs Spending Score)
3. **Cluster Optimization** - Using Elbow Method and Silhouette Score to find optimal cluster count
4. **Algorithm Comparison** - Implementing and comparing K-Means, Hierarchical, and DBSCAN
5. **Business Analysis** - Interpreting clusters and providing actionable recommendations

## 🎯 Marketing Recommendations

### Segment-Specific Strategies

- **Premium Shoppers**: VIP experiences, luxury brand partnerships, exclusive events
- **Standard Shoppers**: Loyalty programs, seasonal campaigns, cross-promotions
- **Fashion-Forward Youth**: Social media marketing, student discounts, trendy products
- **Affluent Conservatives**: Quality-focused messaging, value propositions, expert consultations
- **Budget Conservatives**: Discount events, practical marketing, essential services

## 📁 Project Structure

```
mall-customer-segmentation/
├── data/
│   └── Mall_Customers.csv
├── mall_customer_segmentation.ipynb
└── README.md
```

## 📝 Results Summary

The analysis successfully identified 5 distinct customer segments with **K-Means and Hierarchical clustering showing strong convergence** (95%+ similarity), validating the natural groupings in the data. DBSCAN showed limitations for this structured dataset due to parameter sensitivity and chaining effects.

**Key Success Metrics:**
- Optimal cluster count: 5 (validated by both Elbow Method and Silhouette Score)
- Silhouette Score: 0.55 (indicating well-separated clusters)
- Business actionability: Clear segment profiles with specific marketing recommendations

## 👤 Author

**Eduardo Mazaro**
- GitHub: [@DevMazaro](https://github.com/DevMazaro)
- Email: dev.mazaro@gmail.com

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
