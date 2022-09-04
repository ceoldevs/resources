# Traditional Machine Learning

## Unsupervised Learning
In unsupervised learning, there are no labels for the examples. 

### Clustering
- **K Means Clustering** : It is an iterative approach where a data point is assigned to the group/cluster whose centroid is closest to it among *K* clusters. Optimal number of clusters is determined by the elbow method.  
https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
https://www.aionlinecourse.com/tutorial/machine-learning/clustering

- **Hierarchical Clustering (Agglomerative)** : It follows a bottom-up approach. We form clusters starting with each point being a cluster and build up based on distance between the data points. Based on number of lines the dissimilarity threshold passes through the dendrogram, optimal number of clusters are determined.  
https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html
https://www.aionlinecourse.com/tutorial/machine-learning/hierarchical-clustering