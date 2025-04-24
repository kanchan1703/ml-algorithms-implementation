**Random Forest Algorithm** <br/>


I implemented a Random Forest classifier from scratch in Python to classify the Wisconsin Breast Cancer Dataset.<br/>

Following is the stepwise description of the implementation:<br/>

Step 1: **Dataset Loading and Data Preprocessing** <br/>
       
I loaded the Wisconsin Breast Cancer Dataset, which consists of 569 samples and 30 features. And, a target variable 'diagnosis' (M for malignant, B for benign).

Removed the features that are irrelevant for the implementation.<br/>

Encoded the target variable to change from a categorical data type to a numeric data type.

And, in the end, split the dataset into 80% training and 20% test dataset.<br/>


Step 2: **Decision Tree Classification** <rb/>

Where, I built a decision tree class to create individual trees, using the GINI inpurity for the splits.<br/>



Step 3: **Random Forest Implementation** <br/>


After the decision tree classification, I implemented the Random Forest Classifier, that combines multiple decision trees using Bootstrapping and feature bagging.

The key parameter and the values I used for them<br/>
 
Number of decision trees: 100<br/>
maximum depth = 10<br/>
minimum samples=2<br/>


Step 4: **Model Training and Evaluation** <br/>

Trained the Random Forest model on the training data and predicted labels for the test set and calculated accuracy.

Achieved a test accuracy equal to 62%.<br/>

*Some important terms to know about:* <br/>


**Random Forest**: An ensemble learning method that combines multiple decision trees to improve prediction accuracy and reduce overfitting.<br/>

**Decision Tree**: A tree-like model that splits data based on feature values to make decisions.<br/>

**Ensemble Technique**: A machine learning approach that combines predictions from multiple models to improve accuracy and stability.<br/>

**Bootstrapping**: Sampling data with replacement to create diverse subsets for each tree.<br/>

**Feature Bagging**: Randomly selecting a subset of features at each split to increase tree diversity.<br/>





*A little note for the reader*:  <br/>

The accuracy (62%) is lower than expected for the dataset.

I plan to improve by adding Feature Scaling and debugging the split logic in the Decision Tree classification.
