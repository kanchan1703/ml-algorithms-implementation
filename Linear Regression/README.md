**Linear Regression**
This folder consists of Linear Regression Implementation from scratch. The implementation has been done separately for both **Simple Linear Regression** and **Multi-linear Regression**.

**1. Simple Linear Regression**
I have implemented simple linear regression step by step using a database that shows salaries based on years of experience. We use the algorithm to predict the salary for a given number of years of experience.<br\>
Below are the steps for implementation:
//Step 1: Importing the libraries like NumPy, Pandas, and Matplotlib and loading the dataset in the jupyter notebook.

Step 2: Data Visualization: A scatter plot to visualize the linear relationship between the independent and dependent features.

Step 3: Gradient Descent Implementation: 
Calculated gradient to optimize a0 and a1 by minimizing the Mean Squared Error(MSE)  for 1000 iterations. 

Step 4: Error Tracking: Stored the error and plotted MSE across iterations for visualization purposes.

Step 5: MSE Calculation: MSE is computed for the custom model’s predictions.
In the end, I also implemented the algorithm using scikit-learn to check or compare the findings.

**2. Multi-linear Regression**

Below is the stepwise description of the implementation done in the jupyter notebook:
Step 1: Library Imports and Dataset Loading in the Jupyter Notebook

Step 2: Categorise Feature Handling: 
Applied One-hot Encoding to the feature “State”, converting the categorical data into binary columns for each category in the column and dropping one to avoid multicollinearity.

Step 3: Feature Separation: 
Separated independent features (X) and dependent features(y) and converted them into NumPy arrays.

Step 4: Feature Scaling: 
Standardized numerical independent features and the dependent variable to ensure Gradient Descent stability.

Step 5: Train-Test Split:
Splitting the data into a training (80%) and a testing(20%) dataset.

Step 6: Custom Model Implementation: 
Defined a multipleLinearRegression class with methods for forward pass, loss computation, weight updates, training, testing, and plotting.

Step 7 Model Training and Evaluation: 
In this step, I trained the model using gradient descent with 200 epochs and a learning rate of 0.001.
Then tested the model on the test set, computed test loss, and plotted training loss over epochs.
