**Support Vector Machine(SVM) Algorithm Implementation**<br/>

This is a repository where I have implemented the **Support Vector Machine (SVM) Algorithm** from scratch, where I used both **Linear** and **RBF kernels** and visualized the results in **PCA** space. <br/>

The implementation has given me a good understanding of how the SVM Linear and RBF Kernels work.<br/>

The stepwise description of the implementation:<br/>

Step 1: **Data Loading and Data Preparation** <br/>
I started by loading the  Red Wine Quality dataset, and converted the  quality scores into a Binary Classification Problem by dividing the quality into the sets Good (quality >=7) and Bad (quality<7).<br/>

Step 2: **Dimensionality Reduction** <br/>
I used **Principal Component Analysis** (PCA) to reduce the data from 11 to 2 principal components.
PCA finds new axes and projects the data on them.<br/>

Step 3: **Kernel Functions** <br/>
I implemented both a Linear and RBF (Gaussian) Kernel:

**Kernel:** Measures similarity between points, allowing SVMs to work in higher-dimensional
spaces.<br/>

Linear Kernel:
REF Kernel: 

Step 4: **SVM Training(SMO)** <br/>
I wrote the SVM training loop using the Sequential Minimal Optimization (SMO) algorithm.<br/>

**Margin:** The distance between the decision boundary and the closest data points

Step 5: **Support Vectors** <br/>
After training, I identified the support vectors. These are
the critical points that define the margin and the decision boundary.<br/>
**Support Vector:** A data point that lies on the margin and influences the decision
boundary


Step 6: **Visualization** 
I plotted the decision boundary in PCA space, showing the data points, the regions predicted
by the SVM, and highlighted the support vectors.

**RESULTS** <br/>
Linear SVM accuracy: **0.86** <br/>
RBF SVM accuracy: **0.87** <br/>


*How I Could Improve Accuracy* <br/>

-Tune hyperparameters like `C` and `gamma` using cross-validation.
- Try using more features (not just the first two PCA components).
- Balance the dataset if classes are imbalanced.
- Experiment with other kernels or models (like ensembles).
- Engineer or select more informative features.


