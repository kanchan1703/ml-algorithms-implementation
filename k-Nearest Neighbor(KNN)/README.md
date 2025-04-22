**k-Nearest Neighbor Algorithm**

I have implemented the k-Nearest Neighbor algorithm in this file from scratch using Python. The algorithm is based on the Supervised Learning technique.

Also called a **lazy learner algorithm** as it does not make any assumption on the underlying data.
KNN algorithm does not actually train the data during the training phase but stores it, and when it gets new data, it classifies that data into a category similar to the new data.

How does it work?
1. First, we select k neighbors.
2. Calculate the Euclidean distance of the k number of neighbors..
3. Among these k neighbors, we count the number of data points in each category and assign the new data points to that category fr which the number is maximum
4. The model is ready.


What did I do in the implementation?
1. Imported the required libraries like NumPy, Pandas, and Matplotlib for numerical operations and data visualization.
   
2. Loaded the dataset and explored the data by viewing sample data, features, and target values.

3. Split the dataset into Training and Testing sets using "train_test_split".

4. KNN Implementation
   a. Calculated the Euclidean Distance
   b. Find the nearest neighbors
   c. Predict class labels

5. Tested Custom KNN
   Predicted and printed results using the implemented KNN for a few test samples.

6. Compared with Sklearn KNN
   Used KNeighborsClassifier from sklearn and compared results with the custom model for 
   verification.


