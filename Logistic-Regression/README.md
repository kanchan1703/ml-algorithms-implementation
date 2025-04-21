**Logistic Regression**<br/>

Logistic Regression is a supervised machine learning algorithm that undertakes binary classification tasks by predicting the probability of an outcome or observation.
The model delivers an outcome limited to two possible outcomes, for example, yes/no (or) 0/1 (or) true/false.

Key Properties of Logistic Regression:
1. Logistic Regression's dependent variable follows Bernoulli Distribution.
2. The prediction is based on Maximum Likelihood.

Types of Logistic Regression:
1. Binary Logistic Regression:
It predicts the relationship between the independent and binary dependent variables (for example, 0/1, true/false)<br/>
2. Multinomial Logistic Regression:
A categorical dependent variable has two or more discrete outcomes in this type of logistic regression.
This implies that it will produce more than two possible outcomes.
3. Ordinal Logistic Regression:
Ordinal logistic regression applies when the dependent variable is in an ordered state (i.e., ordinal). 
The dependent variable (y) specifies an order with two or more categories or levels.


Important terms to look at in Logistic Regression:

1. Standardization: 
 Process of scaling data around the mean with a unit standard deviation. 

2. Sigmoid Function: 
In linear regression, we use the hypothesis function (y=ax+b), the linear combination of parameters for a single parameter dataset.
But, in Logistic regression, the responses are not continuous but categorical in 'yes' and 'no' form.
So, we use the sigmoid function to limit the results in between [0,1].

3. Cost Function: 
Cost function or loss function is the function that describes how much the calculated value deviates from the actual value.

4. Gradient Descent:
Gradient descent is an optimization algorithm that is responsible for the learning of best-fitting parameters.
By differentiating the cost function, we get the gradient descent expression.

