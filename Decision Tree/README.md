
**Decision Tree**<br/>

**What did I do in the Decision Tree Implementation?** <br/>

I have implemented Decision Tree Classifier from scratch using NumPy and various other libraries for plotting and visualization etc. 
I encoded the categorical variables using Label Encoder.

Used Information Gain (Entropy) as the splitting criterion, and visualized the predictions with the help of a confusion matrix.<br/>

Also, plotted the Decision tree graphically using Graphviz.

Achieved **100% accuracy** on the test set for the provided drug dataset, with all classes
correctly classified and no misclassifications


**A little bit about the Decision Tree Classifier**<br/>

Decision tree is a Supervised Learning technique that can be used both for classification and regression.
A tree structure, where the internal nodes represent features of a dataset. Branches represent the decision nodes and leaf nodes represent the outcomes.

**Decision Node** (problem node): is used to make decisions and has multiple branches

**Leaf Node** (solution node): is the outcome of the decision nodes. These nodes do not contain further branches.

The decision tree is based on **CART (Classification and Regression Technique)** algorithm, which is used of both classification and regression. 
***CART algorithm works by recursively partitioning the training data into smaller subsets using binary splits.***

**Why or when do we use a decision tree?** <br/>

-Decision trees are easy to understand and interpret.
- They mimic human decision-making logic.
- They can handle both numerical and categorical data.

**How does it work?** <br/>

1. Start with root node S containing the entire dataset.

2. Select the best attribute using Attribute Selection Measure (ASM).

3. Split S into subsets based on possible values of the best attribute.

4. Create a decision tree node with the best attribute.

5. Recursively build new decision trees for each subset until nodes cannot be further classified, designating them as leaf nodes

**Attribute Selection Measure**
ASM is a technique which is used to select the best attribute for the root node and for the sub-nodes.

The two popular ASM techniques are :<br/>

1. **Information gain**
Information gain is the measurement of changes in entropy after the segmentation of a dataset based on an attribute.

*Information Gain= Entropy(S)- [(Weighted Avg) *Entropy(each feature)*

The node with maximum Information Gain is used for splitting.

**Entropy**: Entropy is a metric to measure the impurity in a given attribute.

*Entropy(s)= -P(yes)log2 P(yes)- P(no) log2 P(no)
P(yes) = probability of 'Yes'
P(NO) = probability of 'No'*

2. **Gini Index**

Gini index is a measure of impurity or purity used while creating a decision tree. Attribute with low Gini Index is used to create the split.

*Gini Index= 1- ∑jPj2*

**A note for the reader**
*This project is a great starting point for anyone who wants to understand how decision trees
work at a low level, without relying on machine learning libraries.*


