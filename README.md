# **Image Classification on MNIST and EMNIST Letters**
The project is to train a deep neural network to classify images on MNIST and EMNIST datasets.

**Summary of Accuracy on MNIST**
- training accuracy: 99.92%
- validation accuracy: 99.60%
- test accuracy: 99.48%

**Summary of Accuracy on EMNIST**
- training accuracy: 98.7%
- validation accuracy: 95.1%
- test accuracy: 94.9%

## Environment and Run Jupyter Notebook

* Tensorflow
* Keras
* Sklearn
* scipy
* numpy
* cv2
* matplotlib

run "image-classification-mnist-emist.ipynb"

## Vanishing Gradient Problem
When training the neural network, during the backpropogation in each subsequent layer, the gradient in earlier layers get exponientially smaller and smaller ([vanishing](https://github.com/zmandyhe/image-classification-mnist-emnist-letters/blob/master/pic/vanishing-gradient.png)), which makes the network learning very little/slow to improve.  

Potential Solutions include:
- Batch normalization, which is to normalize the activations of the previous layer at each batch, i.e. applies a transformation that maintains the mean activation close to 0 and the activation standard deviation close to 1 to reduce the oscillations of in the distribution of activation. Deep network can be trained faster and better when the activation is normalized during backpropogation.
- Use ReLu activation will normally solve the vanishing gradient problem (not sigmoid).
- Using Regularization to modify cost function to penalize larger weights.
- Use different weight initialization, mementum, etc.
- Use more data.
- Modify architecture.


## References
* Michael Nielsen's [Neural Network and Deep Learning](http://neuralnetworksanddeeplearning.com/)
* [Batch Normalization: Accelerating Deep Network Training by Reducing Internal Covariate Shift](https://arxiv.org/abs/1502.03167)
* [Stanford course on Convolutional Neural Networks for Visual Recognition](http://cs231n.github.io/neural-networks-1/#actfun)
