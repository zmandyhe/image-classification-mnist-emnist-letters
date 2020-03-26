# **Image Classification on MNIST and EMNIST Letters**
The project is to train a deep neural network to classify images on MNIST and EMNIST datasets.

## Environment

* Tensorflow
* Keras
* Sklearn
* scipy
* numpy
* cv2
* matplotlib

## Vanishing Gradient Problem
When training the neural network, during the backpropogation in each subsequent layer, the gradient in earlier layers get exponientially smaller and smaller (vanishing), which makes the network learning very little/slow to improve.  
![Vanishing Gradient](https://github.com/zmandyhe/image-classification-mnist-emnist-letters.git/blob/master/pic/vanishing-gradient.png)

Potential Solutions include:
- Batch normalization, which is to normalize activations for each layer in between. 
- Choose the right activation function. Rather Sigmoid, choosing ReLu will reduce the chance of having the vanishing gradient problem.
- Using Regularization
- Use different weight initialization, mementum, etc.
- Use more data.
- Modify architecture.

## Dead ReLu Problem

## Strategy to Avoid Overfitting

## References
* Michael Nielsen's [Neural Network and Deep Learning](http://neuralnetworksanddeeplearning.com/)
