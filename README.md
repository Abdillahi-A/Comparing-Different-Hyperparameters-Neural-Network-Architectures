# Comparing-Different-Hyperparameters-Neural-Network-Architectures

## Goal

This project explores three neural network architectures: 
1) single layer perceptron
2) multilayer perceptron and;
3) convolutional neural network. 

It does so by altering a number of hyper-parameters in each network and comparing the impact of these alterations to the various networks’ performance in recognizing handwritten digits provided by the MNIST dataset.


## Result

Of all three neural network architectures, CNN had the highest performance in recognising handwritten digits from the MNIST dataset with a test accuracy of 98.13%. This was followed by the MLP architecture with model_5c achieving a test accuracy of 96.74%. The lowest performer was the SLP with model_1c achieving a test accuracy of 92.36%. In terms of hyperparameters, learning rate seemed to be the most sensitive hyperparameter, with minor adjustments in either direction of 0.001 leading to drops of up to 77% in accuracy. 
Choice of activation had the 2nd biggest effect on model performance, with switching from sigmoid to relu resulting in an increase of 2.7% in test accuracy. The next most influential hyperparameter was batch size, which was negatively correlated with accuracy such that an increase in batch size from 128 to 512 resulted in a 0.93% reduction in test accuracy. Number of hidden layers in the network was positively correlated with performance such that more hidden layers increased test accuracy, however, this relationship occurred at a decreasing rate, suggesting that increasing layers beyond a certain point may not yield much in terms of improved accuracy. Number of epochs were positively correlated with performance, however a few models had issues with overfitting with particularly high epochs. Interestingly, relu and tanh would begin to overfit at much sooner epochs than sigmoid. Number of nodes seemed to have a small, albeit negative correlation with performance, such that an increase from 32 nodes to 128 nodes saw a 0.39% decrease in test accuracy.  

