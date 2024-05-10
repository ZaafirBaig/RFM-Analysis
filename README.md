# RFM Analysis

## Overview
This repository contains code for performing RFM (Recency, Frequency, Monetary) analysis on a dataset. RFM analysis is a technique used in marketing to segment customers based on their transaction history. It helps in identifying and targeting specific customer groups for personalized marketing strategies.

## Dataset
The dataset used in this analysis contains information about sales transactions from a superstore. It includes columns such as Order Date, Segment, Country/Region, City, Region, Category, Sub-category, Sales, Quantity, Discount, and Profit.

## Analysis
### Elbow Method
- The Elbow Method was used to determine the optimal number of clusters for customer segmentation based on RFM variables.
- A KMeans clustering algorithm was applied to group customers into different clusters.
- The optimal number of clusters was determined to be 4 based on the Elbow Method.

### Cluster Visualization
- Descriptive statistics were calculated for each cluster, including mean and standard deviation, to understand the characteristics of each segment.
- Visualizations such as histograms and line graphs were created to explore the distribution of RFM variables within each cluster.
- The clusters were interpreted and categorized based on their RFM characteristics.

### Calinski-Harabasz Criterion
- The Calinski-Harabasz criterion was used as an additional evaluation metric for determining the optimal number of clusters.
- A curve was plotted showing the Calinski-Harabasz score for different values of K.
- The curve showed an increase until K=7, a drop at K=8, and then an increase after that.

### Davies-Bouldin Index
- The Davies-Bouldin Index was calculated as another measure of cluster quality.
- The index value was determined to be 0.579, indicating a moderate level of separation between clusters.

## Repository Structure
- **RFM_Analysis.ipynb**: Jupyter Notebook containing the code for RFM analysis.
- **README.md**: This file, providing an overview of the project.
- **data/**: Directory containing the dataset used in the analysis.

## Dependencies
- Python 3
- Jupyter Notebook
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, yellowbrick
