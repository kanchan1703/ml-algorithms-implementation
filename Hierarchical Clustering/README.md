**Hierarchical Clustering Algorithm** <br/>

Hierarchical clustering is an **unsupervised learning** method, also known as *hierarchical cluster analysis*, which groups similar objects into clusters.<br/>

A hierarchical clustering approach is based on determining successive clusters based on previously defined clusters. The main aim is to group the similar data points into a hierarchy or tree-like structure called **dendrograms**.<br/>


**Dendrogram**: A dendrogram is a family tree of clusters, which shows how data points or groups of data merge together.<br/> The bottom shows each data point as its own group, and as you move up, similar groups are combined. The lower the merge point, the more similar the groups are. <br/>



**Types of Hierarchical Clustering** <br/>

1. Agglomerative Clustering (bottom-up approach)<br/>
2. Divisive Clustering (top-down approach)  <br/>




**Implementation of Agglomerative Hierarchical Clustering** <br/>

I implemented *Agglomerative Hierarchical Clustering*, using the *Stock Price* dataset in python from scratch.<br/>


*What exactly is **Agglomerative** Hierarchical Clustering?* <br/>

This is a *bottom-up* approach, where each observation starts in its cluster, and pairs of clusters are merged as one moves up the hierarchy. <br/>

On each iteration, we will merge the least dissimilar clusters (most similar).<br/>

The dissimilarity will denote the depth of the tree, and we can calculate the dissimilarity using *Euclidean distance* method.
The distance between clusters can be solved by **Linkage**.<br/>

There are 4 types of linkages:<br/>

1. Complete Linkage. Calculates all pairwise measures for observations in clusters and returns the largest of those values.<br/>
2. Single Linkage. Minimum distance is recorded from all pairwise measures.<br/>
3. Average Linkage. Records the average of all pairwise distances.<br/>
4. Ward Linkage<br/>


In the implementation, I preprocessed the dataset by *Feature Selection*, where I selected numerical features for the implementation and then *Standardized* the dataset to *Normalize* the features, ensuring equal contribution to distance calculations for clustering.<br/>

After that I defined the **Hierarchical Clustering Class**, where I defined **Euclidean Distance** and **Cluster Distance**. <br/>

In the **Fit Method**, built linkage matrix is built by iteratively merging the closest clusters, storing the merging details. <br/>

At the end of the implementation, I plotted the **Dendrogram**, visualizing the clustering hierarchy and **Cluster** Scatter Plot in 2D using two features *Current Price* and *Volatility*. <br/>

This implementation provides a custom, interpretable approach to hierarchical clustering, suitable for analyzing stock data patterns.










