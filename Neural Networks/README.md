**Neural Network Algorithm**

Neural networks are machine learning models inspired by the human brain's interconnected neuron structure.<br/>

A neural network consists of **neurons**, which are the fundamental units, just like the brain cells. These neurons receive inputs, process them, and produce an output.<br/>

The neural networks structured into distinct layers, an *Input Layer*, *Hidden Layer* and the *Output Layer*.<br/>
**Input Layer**: This layer receives the data.<br/>
**Hidden Layer**: The layer processes the data by gradually improving its performance by adjusting weights and biases. A neural network can have multiple hidden layers.<br/>
**Output Layer**: It provides the final decision or predictions.<br/>


**Why do we need Neural Networks?** <br/>

Neural Networks are pivotal in identifying complex patterns and solving complex challenges.<br/>

Their ability to learn from the vast amount of data and been very impactful in technologies like
**NLP (Natural Language Processing)**, **Self-driving Vehicles** and many more. <br/>

There are several different types of neural networks, We generally focus on the following:<br/>

1. **Multilayer Perceptrons (MLPs)**: The classical type of neural network with one or more layers of neurons.<br/>

2. **Recurrent Neural Networks (RNNs)** are designed to work with sequence prediction problems such as One-to-Many, Many-to-One and Many-to-Many.<br/>

3. **Convolutional Neural Networks (CNNs)** are designed to map image data to an output variable, proven to be a go-to method for prediction problems involving image data as input.<br/>


I have implemented MLP Neural Network, where I used the Python library for my implementation from scratch.<br/>

*What exactly is a Multi-Layer Perceptron?* <br/>

A neural network, which consists of at least 3 layers, input, one or more hidden and and output layer. Each neuron in one layer is connected to every neuron in the next layer.<br/>

An MLP learns by adjusting the weights and minimizing the error of its predictions, using the backpropagation process.<br/>

I loaded the dataset and then did the necessary preprocessing and defined the **MLP class**, where I initiated the parameters and then implemented the **Activation Function**.<br/>

This MLP class implements a simple MLP with one hidden layer, **ReLU activation**, and binary
**cross-entropy loss**.<br/>

Activation Functions:<br/>
**ReLU** is used in the hidden layer for non-linearity, **sigmoid** in the output for binary
classification.<br/>

*Backpropagation*: Computes gradients of the loss function for each weight.<br/>
*Gradient Descent*: Updates weights to minimize the loss function.<br/>

The model is trained over 100 epochs, and the test accuracy is printed, which is 0.62.
This plot shows how the training loss decreases over epochs, indicating learning progress.<br/>

To improve the test accuracy, I used different values for the parameters, and we could see the change in the Loss curve in the second plot.



