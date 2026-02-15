# MSCS_634_Lab_3  
## Clustering Analysis Using K-Means and K-Medoids  

### Overview  
This lab explores unsupervised learning techniques using the Wine dataset from the sklearn library. The objective was to apply and compare two clustering algorithms — K-Means and K-Medoids — using k = 3 (since the dataset contains three natural classes). After standardizing the dataset, both algorithms were evaluated using the Silhouette Score and Adjusted Rand Index (ARI). Visualizations using PCA were created to compare clustering structures.

---

## Purpose of the Lab  

The purpose of this lab was to:

- Understand how clustering algorithms group unlabeled data.
- Implement K-Means and K-Medoids on a real-world dataset.
- Evaluate clustering quality using Silhouette Score and ARI.
- Visually compare cluster structures using dimensionality reduction.
- Reflect on when each clustering method is more appropriate.

---

## Key Insights from Clustering Results  

- **K-Means achieved higher performance** with:
  - Silhouette Score: 0.2849  
  - ARI: 0.8975  

- **K-Medoids showed slightly lower performance** with:
  - Silhouette Score: 0.2676  
  - ARI: 0.7411  

- The higher ARI for K-Means indicates stronger agreement with the true class labels.
- PCA visualizations showed that K-Means formed more compact and well-separated clusters.
- K-Medoids, while slightly less accurate, provides robustness against outliers because it selects actual data points as cluster centers.

Overall, the Wine dataset appears well-suited for K-Means due to its relatively structured and compact cluster distribution.

---

## Challenges and Decisions  

- Ensuring proper data standardization was essential, as clustering is distance-based.
- Installing and importing `scikit-learn-extra` was necessary for implementing K-Medoids.
- PCA was used to reduce dimensionality for visualization while preserving cluster structure.
- Care was taken to evaluate models using both internal (Silhouette Score) and external (ARI) metrics for a comprehensive comparison.

---

## Conclusion  

This lab demonstrated that while both K-Means and K-Medoids can effectively cluster the Wine dataset, K-Means produced better-defined clusters in this case. The results highlight how dataset characteristics influence clustering performance and reinforce the importance of evaluation metrics when comparing algorithms.

---



