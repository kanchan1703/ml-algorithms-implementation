**Naive Bayes Algorithm**

In this file, I implemented the Naive Bayes algorithm from scratch. The algorithm is based on applying Bayes' Theorem with a  strong independence assumption between the features, where it predicts probabilities for each class, and the class with the highest probability is considered the most likely class.
This is known as **MAP (Maximum A Posteriori)**

MAP(A)
= max (P (A | B))

= max (P (B | A) * P (A))/P (B)

= max (P (B | A) * P (A))

**Types of Naive Bayes Algorithm**
1. Gaussian Naive Bayes
2. Multinomial Naive Bayes
3. Bernoulli Naive Bayes

I have mainly concentrated on the **Gaussian Naive Bayes Algorithm** in the implementation.

Since the data consists of continuous attribute values, it is assumed that the class is Normal/Gaussian distributed.

Some of the applications of Naive Bayes Algorithms:
1. Spam filtering
2. Text classification
3. Sentiment analysis
4. Recommendation System

**Steps I followed in the implementation:**

1. Maths behind the implementation
   a. Implemented Bayes' Theorem
   b. Demonstrated the Independence assumption
   c. used Gaussian PDF (probability density function) for Likelihood Estimation

2. Model Implementation:
   a. Fit (X, y) and computed Mean, Variance, Class Prior
   b. Predicted 'X' to compute posterior probabilities
   c. used 'Log' to improve numerical stability

3. Model Evaluation
   a. Evaluated predictions like  Accuracy, Recall and F1-Score
   b. Used the Confusion Matrix for visualization







