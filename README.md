# Cluster-ATM-withdrawal-behaviors-to-detect-unusual-activity.
Welcome to the repository for Clustering Methods and Financial Insights. This project explores three popular clustering algorithms—K-Means, DBSCAN, and Gaussian Mixture Models (GMM)—to analyze transactional data, withdrawals specifically and derive actionable business decisions.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Project Overview**

This repository provides an end-to-end implementation of clustering techniques on financial datasets to identify distinct patterns of behavior and anomalies. The clustering outcomes serve as a foundation for business decision-making, including risk management, fraud detection, and customer segmentation.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Clustering Techniques Used**

K-Means Clustering:
Partitions the dataset into a predefined number of clusters using a centroid-based approach.
Suitable for identifying well-separated groups in transactional data.

DBSCAN (Density-Based Spatial Clustering of Applications with Noise):
Identifies clusters based on the density of points in the feature space.
Effectively detects noise and anomalies, making it ideal for fraud detection.

Gaussian Mixture Models (GMM):
A probabilistic clustering algorithm that assigns probabilities to data points for belonging to multiple clusters.
Handles overlapping clusters and offers nuanced insights into financial data.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Fallout**

Anomaly Detection (DBSCAN):
Identify high-risk or potentially fraudulent transactions by analyzing noise points.
Use outlier insights to bolster risk mitigation strategies in financial processes.

![image](https://github.com/user-attachments/assets/95ac1f14-c4a4-4796-8177-fb77ae0038e6)



Customer Segmentation (K-Means):
Segment customers into high-value and low-value groups for targeted marketing strategies.
Separate routine transactions from outliers, helping refine operational processes.

![image](https://github.com/user-attachments/assets/92e0f844-be6f-4537-9de4-131f0d41a4eb)



Behavioral Insights (GMM):
Understand overlapping behaviors, such as customers transitioning between high-risk and stable activities.
Use probabilistic cluster assignments to enhance decision-making in credit scoring and personalized offerings.

![image](https://github.com/user-attachments/assets/ac756172-554c-4f7b-9ff8-1c6045fa7f09)


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Comparison Table**

Explaining the Clusters
Clusters represent groups of similar data points based on the input features. They highlight patterns, behaviors, or characteristics that group certain data points together. Here's what the clusters might mean in practical terms:

Cluster 0:
Represents moderate withdrawal activity with medium balances.
This cluster may correspond to customers with stable financial habits who conduct regular, routine transactions.

Cluster 1:
Characterized by high withdrawal amounts and negative balances.
This could flag high-risk accounts, possibly due to excessive spending, overdrafts, or other unusual financial behaviors.

Cluster 2:
Comprises low withdrawal amounts and positive balances.
Likely represents low-risk, financially stable customers who maintain sufficient balances.
By analyzing these clusters, businesses can tailor financial services, flag unusual activities for deeper review, or strategize targeted engagement campaigns.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Why GMM is the Best Model**

1. Flexibility in Cluster Shape
GMM assumes that each cluster is a Gaussian distribution, allowing for overlapping, irregular, or varying cluster shapes.
Unlike K-Means, which enforces rigid, spherical clusters, GMM provides a nuanced clustering solution. This flexibility is ideal for datasets where clusters have different spreads or orientations.

2. Probabilistic Clustering
GMM assigns probabilities for each point belonging to a cluster, rather than hard boundaries.
This means that data points on the edges of clusters are not forced into a single cluster but have a likelihood of belonging to more than one. This soft clustering approach reflects real-world data behaviors more accurately.

3. Robustness to Overlaps
Compared to DBSCAN, which depends heavily on parameters like eps (radius) and struggles with overlapping or close-together clusters, GMM handles overlaps gracefully.
For example, if two customer types share similar behaviors but differ subtly (e.g., frequent withdrawals in different transaction ranges), GMM can delineate them probabilistically.

4. Performance and Cohesion
The silhouette score for GMM was 0.7613, the highest of the three, indicating:
Cohesion: Points within each cluster are closely related.
Separation: Clusters are distinct from each other.
This confirms that GMM captured the underlying structure of the data better than K-Means (0.5955) and DBSCAN (0.4557).

<img width="525" alt="image" src="https://github.com/user-attachments/assets/108dc8e8-7238-438e-baed-26552489c882" />
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
