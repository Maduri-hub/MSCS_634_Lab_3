# MSCS 634 - Lab 3: Clustering Analysis

## Purpose
This lab explores clustering techniques using the Wine dataset from sklearn. 
K-Means and K-Medoids algorithms were implemented and compared using evaluation metrics.

## Dataset
The Wine dataset was loaded from sklearn.datasets. 
The dataset contains 178 samples with 13 numerical features and 3 target classes.

## Methods
- Data standardization using z-score normalization.
- K-Means clustering with k=3.
- K-Medoids clustering with k=3.
- Evaluation using Silhouette Score and Adjusted Rand Index (ARI).
- PCA used for 2D visualization.

## Key Results
- Compared Silhouette Scores to measure cluster separation.
- Compared ARI to evaluate similarity to true class labels.
- Observed differences between centroid-based and medoid-based clustering.

## Observations
- K-Means tends to form spherical clusters.
- K-Medoids is more robust to outliers since medoids are actual data points.
- The model with higher Silhouette and ARI performed better overall.

## Challenges
- Python 3.14 compatibility issue with sklearn-extra.
- Implemented K-Medoids manually using the PAM approach.
