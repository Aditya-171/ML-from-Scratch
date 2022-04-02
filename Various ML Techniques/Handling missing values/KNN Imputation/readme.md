## Knn Imputation
---

K-nearest neighbour (KNN) imputation is an example of neighbour-based imputation.For a discrete variable, KNN imputer uses the most frequent value among the k nearest neighbours and,
for a continuous variable, use the mean or mode. 

By default, a euclidean distance metric that supports missing values, nan_euclidean_distances, 
is used to find the nearest neighbors. Each missing feature is imputed using values from n_neighbors nearest neighbors
that have a value for the feature. The feature of the neighbors are averaged uniformly or weighted by distance to each neighbor. 

If there are more many nan values in the dataset then we can use nan_euclidean_distances for calculating the distane.
Compute the euclidean distance between each pair of samples in X and Y, where Y=X is assumed if Y=None. When calculating the distance between a pair of samples, this formulation ignores feature coordinates with a missing value in either sample and scales up the weight of the remaining coordinates:

dist(x,y) = sqrt(weight * sq. distance from present coordinates) where, weight = Total # of coordinates / # of present coordinates

For example, the distance between [3, na, na, 6] and [1, na, 4, 5] is: sqrt( (4/2) [(3-1)**2 + (6-5)**2]  )
 


 

