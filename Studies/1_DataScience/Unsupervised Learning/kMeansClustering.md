The kMeansClustering is an algorithm in unsupervised learning used for clustering not labeled instances, the problem can be describe as: imagining a not labeled dataset, then i need to give those instances a label. 
- The kMeans will do this by positioning **k** centroids (that represent the number of clusters).
- Each instance then is associated to the nearest centroid.
- In these step the algorithm re-calculate the centroid from each cluster based on the current average position of the cluster members.
- The steps 2 and 3 repeat iteratively, until the algorithm obtain the ideal position for the centroids.

![[kmeans-animated.gif]]
