# k-means-algorithm
This is a Python implementation of k-means algorithm including elbow method and silhouette method for selecting optimal K

K-means is a popular clustering algorithm used for partitioning data into K clusters. It works by iteratively assigning each data point to the nearest cluster centroid and then recalculating the centroid of each cluster based on the data points assigned to it. The process is repeated until convergence.

# Algorithm
* Randomly select K initial cluster centroids from the data points.
* Assign each data point to the nearest cluster centroid.
* Recalculate the centroid of each cluster based on the data points assigned to it.
* Repeat steps 2-3 until convergence (i.e. when the cluster assignments no longer change).
## Objective Function
The objective of k-means is to minimize the sum of squared distances between each data point and its assigned cluster centroid. The objective function can be written as:
$$ minimize J = ∑i=1 to n ∥ xi - μj ∥^2$$

# Elbow Method
The Elbow method is a heuristic used to determine the optimal number of clusters in K-Means clustering. The method plots the sum of squared distances between each observation and its assigned centroid as a function of the number of clusters. The "elbow" point on the plot indicates the number of clusters where adding additional clusters does not result in significant reduction in the sum of squared distances.

The Elbow method can be summarized by the following steps:

* Run K-Means clustering for a range of k values
* Calculate the sum of squared distances for each k value
* Plot the sum of squared distances as a function of k
* Identify the "elbow" point on the plot


# Silhouette Method
The Silhouette method is another heuristic used to determine the optimal number of clusters in K-Means clustering. The method measures the quality of each observation's cluster assignment by calculating its silhouette coefficient. The silhouette coefficient ranges from -1 to 1, where a value of 1 indicates that the observation is well-clustered and a value of -1 indicates that the observation is misclassified.

The Silhouette method can be summarized by the following steps:

* Run K-Means clustering for a range of k values
* For each observation, calculate the silhouette coefficient
* Calculate the average silhouette coefficient for each k value
* Plot the average silhouette coefficient as a function of k
* Identify the k value with the highest average silhouette coefficient
