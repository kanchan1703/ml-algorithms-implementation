**k-Means Clustering Algorithm** <br/>

k-Means Clustering is an **Unsupervised Machine Learning Algorithm** that divides the **unlabeled dataset**(data without defined categories) into 'k' different clusters.<br/>
The algorithm works iteratively to assign each data point to one of K groups based on the provided features. Data points are clustered based on feature similarity.<br/>

*An **unsupervised model** has independent variables with no dependent variables.*<br/>


**What exactly is the k-Means Clustering Algorithm?** <br/>

It is a **Centroid-based algorithm**, where each cluster is associated with a centroid. The main goal is to minimize the distance between the data points and their related cluster.<br/>

The two main tasks the algorithms focus on are:<br/>
1. to determine the best value for k center points or centroids <br/>
2. Assigning each data point to its closest k-center, to create a cluster.<br/>


**Why use k-Means?**

k-Means is a powerful and efficient tool yet the simplest clustering algorithm of all, it is used to uncover patterns and structures by grouping similar data points into clusters. <br/>

Some of the use cases are:<br/>
Behavioral segmentation<br/>
Inventory categorization<br/>
Sorting the Sensor measurements<br/>
Stock Market Analysis <br/>

I implemented K-Means Clustering algorithm from scratch using Python. I used the stock dataset, where stocks of different price ranges are given, and I clustered them according to their prices.<br/>

Firstly, I loaded the dataset and preprocessed the data to make it suitable for clustering, by removing the irrelevant features and cleaning the dataset, and standardizing the features so that all the features have equal effect on the implementation of the model.

After the preprocessing of data, I defined the *Euclidean Distance* function and chose the centroids with th the help of **Elbow Method** <br/>

Choosing the right number of clusters (k) is a key step in K-means clustering. I used the Elbow method to do the same.<br/>

**Euclidean Distance**: It measures the straightest and shortest path between two points. Here, the distance is between the data points from each centroid.<br/>

**Elbow Method**: One of the most used methods, we run K-means clustering for a range of k values (e.g., from 1 to 10). <br/>
For each k, calculate the *Within-Cluster Sum of Squares (WCSS)*, also called *inertia*. This measures how tightly the data points are clustered around the centroids. Then we plot k vs WCSS, and the “elbow” point in the plot, where the rate of decrease sharply slows. This point is often a good choice for k.<br/>

In the plot, the curve bends at **k=3**, so we take that many number of centroids. And, then we plot the k-Means plot for k=3 and k=4 to compare how each plot looks.







