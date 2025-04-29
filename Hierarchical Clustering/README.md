**Hierarchical Clustering Algorithm** <br/>

Hierarchical clustering is an **unsupervised learning** method, also known as *hierarchical cluster analysis*, which groups similar objects into clusters.<br/>
A hierarchical clustering approach determines successive clusters based on previously defined clusters. The main aim is to group the similar data points into a hierarchy or tree-like structure called **dendrograms**.<br/>

**Dendrogram**: A dendrogram is a family tree of clusters, which shows how data points or groups of data merge together.<br/> The bottom shows each data point as its own group, and as you move up, similar groups are combined. The lower the merge point, the more similar the groups are.
<br>                                                                                                                                                                                                                                             
**Types of Hierarchical Clustering**
<br>
1. Agglomerative Clustering (bottom-up approach)
2. Divisive Clustering (top-down approach)  

<br>

**Implementation of Agglomerative Hierarchical Clustering** 

I implemented *Agglomerative Hierarchical Clustering*, using the *Stock Price* dataset in Python from scratch.

<br>

*What exactly is **Agglomerative** Hierarchical Clustering?* 
<br>
This is a *bottom-up* approach, where each observation starts in its cluster, and pairs of clusters are merged as one moves up the hierarchy.
<br>
We will merge the least dissimilar clusters (most similar) on each iteration.
The dissimilarity will denote the depth of the tree, and we can calculate the dissimilarity using *Euclidean distance* method.
The distance between clusters can be solved by **Linkage**.
<br>
*There are 4 types of linkages*: 
1. Complete Linkage. Calculates all pairwise measures for observations in clusters and returns the largest of those values.<br/>
2. Single Linkage. Minimum distance is recorded from all pairwise measures.<br/>
3. Average Linkage. Records the average of all pairwise distances.<br/>
4. Ward Linkage<br/>

<br>

In the implementation, I preprocessed the dataset by dropping the categorical features and unnecessary features, since they won't be appropriate for clustering.
<br>
After that, I defined the **Hierarchical Clustering Class**, where I defined **Euclidean Distance** and **Cluster Distance**, and then calculated the minimum distance between non-diagonal values, which tells us about the closest clusters.
<br>
In the **Fit Method**, built linkage matrix is built by iteratively merging the closest clusters, storing the merging details.
<br>
After that, building the Hierarchical cluster and assigning cluster labels by the **Predict Method**.

<br>


At the end of the implementation, I plotted the **Dendrogram**, visualizing the clustering hierarchy and **Cluster** Scatter Plot in 2D using two features. 
<br>
I used the first **30 samples** to plot the dendrogram to make it less cluttered.
<br>
This implementation provides a custom, interpretable approach to hierarchical clustering, suitable for analyzing stock data patterns.

<br>

**How is Hierarchical Clustering different from k-Means Clustering?** <br/>
Unlike K-Means, it does not need a pre-defined number of clusters. <br/>
K-Means is a division of the dataset into non-overlapping subsets, whereas Hierarchical clustering is a set of nested clusters arranged in the form of a tree.<br/>

<br>


**Some real-life uses of Hierarchical Clustering**
Hierarchical clustering has a wide range of applications across various domains. Such as:
1. Customer Segmentation: segmenting customers based on their purchasing preferences and behavior.<br/>
2. Recommender Systems: Hierarchical clustering can assist in building recommender systems by grouping similar users or items based on their preferences or behavior. <br/>
3. Gene Expression Analysis: used to identify patterns and clusters of genes with similar expression profiles, which can helo in understanding gene relationships.











