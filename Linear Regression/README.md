**Linear Regression**
Linear Regression is a statistical method used to derive the relationship between a dependent variable(target) and one or more independent variables (predictors).<br/> It is widely used for prediction, forecasting and understanding variable relationships.<br/> 
This folder consists of Linear Regression Implementation from scratch. The implementation has been done separately for both **Simple Linear Regression** and **Multi-linear Regression**.


**1. Simple Linear Regression**
It involves one independent variable (for ex: predicting house price based on size)<br/>
I have implemented simple linear regression step by step using a database that shows salaries based on years of experience. We use the algorithm to predict the salary for a given number of years of experience.<br/>
Below are the steps for implementation:<br/>

Step 1: Importing the libraries like NumPy, Pandas, and Matplotlib and loading the dataset in the jupyter notebook.

Step 2: Data Visualization: A scatter plot to visualize the linear relationship between the independent and dependent features.

Step 3: Gradient Descent Implementation: 
Calculated gradient to optimize a0 and a1 by minimizing the Mean Squared Error(MSE)  for 1000 iterations. 

Step 4: Error Tracking: Stored the error and plotted MSE across iterations for visualization purposes.

Step 5: MSE Calculation: MSE is computed for the custom model’s predictions.<br/>
In the end, I also implemented the algorithm using scikit-learn to check or compare the results of the implementation and the actual library.

**2. Multi-linear Regression**<br/>

It involves multiple independent variables (for example, predicting house prices based on multiple factors like size, location and number of bedrooms)
Below is the stepwise description of the implementation done in the jupyter notebook:<br/>

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

**Real-Life Applications of Linear Regression**
Linear regression is widely used in the tech industry due to its simplicity, interpretability, and efficiency.<br/>
It has numerous industrial applications such as predicting sales, analyzing risk, analyzing customer behavior and optimizing processes.<br/>
Here are some specific industrial applications:<br/>
1. Finance:<br/> It is used for predicting stock prices and forecasting economic trends and assessing potential financial risks.<br/>
2. Marketing: <br/> We can use linear regression in the field of marketing to predict sales and analyze customer behavior.<br/>
3. Risk Assessment:<br/> Estimating costs of insurance claims, evaluating financial risks, and making informed decisions about risk taking. <br/>
Other industries where linear regression is effectively used are healthcare, engineering, supply chains etc.

