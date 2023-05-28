# K Means Clustering Implementation In Python

## Documentation

### Attributes

`KMeans(self, n_clusters = 3, tolerance = 0.01, max_iter = 100, runs = 1, init_method="forgy")`

`n_clusters`: Number of clusters

`tolerance`: Tolerance value. Algorithm stops if distance between previous centroids and current centroids is less than tolerance.

`max_iter`: Number of iterations in every run.

`runs`: Determines how many times the algorithm will run. Makes sense only if random initialization method is used. Therefore disregarded when a non-random initialization method is chosen.

`init_method`: Initialization method. Only four methods implemented: Forgy, Macqueen, Maximin, Var-Part

Macqueen simply selects first K obversation and assigns them as centroids.

Forgy takes K random data points as initial centroids

Maximin and Var-Part are more sophisticated initialization methods. Var-Part is usually more efficient. Link to their related papers are in the section below.

`KMeans.fit(X)`: Runs the K Means algorithm.

