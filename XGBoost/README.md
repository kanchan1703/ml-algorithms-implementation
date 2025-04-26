**XGBoost Algorithms Implementation** <br/>

XGBoost is  a type of **ensemble learning** method, which is an optimized implementation of **Gradient Boosting**.<br/>


To better understand XGBoost algorithm we need to better understand about Gradient Boosting.<br/>

**Ensemble Learning**: Ensemble learning combines multiple weak models to form a stronger model. <br/>

**Gradient Boosting**: an ensemble learning method used for both classification and regression tasks.<br/>
It is a boosting algorithm which combine multiple weak learner to create a strong predictive model.<br/>
In gradient boosting, each new model is trained to minimize the **Loss Function** (mean squared error) (or) **Cross-Entropy** of the previousmodl using **Gradient Descent**.<br/>


I implemented the model by scratch using Python.<br/>

I started by loading the dataset and doing the basic EDA (Exploratory Data Analysis).<br/>

Steps I followed to implement XGBoost from scratch: <br/>

1. **Gradient and Hessian Calculation**: For each boosting round, I calculated *Gradient* (first derivative) and *Hessian* (second derivative) of the loss function for tree construction. <br/>

**Boosting**: It is an ensemble machine learning technique that combines multiple weak learners (typically shallow decision trees) to create a strong predictive model. The core idea is to train models sequentially, where each new model focuses on correcting the errors made by the previous ones. <br/>


2. **Greedy Split Search**: For each node, all possible splits are evaluated using gain/loss reduction criteria. <br/>

3. **Tree Construction**: Decision trees are constructed recursively using the best splits, with regularization and early stopping to prevent overfitting. <br/>

4. **Leaf Value Calculation**: Optimal leaf weights are computed using aggregated gradients and Hessians, incorporating L2 regularization. <br/>

5. **Ensemble Aggregation**: Trees are sequentially added, each correcting the residuals of the previous ensemble, following the gradient boosting paradigm. <br/>


After this, I trained the model on the training set, iteratively fitting trees to minimize the objective function. <br/>

Then, I used the trained model to generate predictions on the test set and evaluated the model using metrics such as *Mean Squared Error* (MSE) and compared the predicted and actual target values.






