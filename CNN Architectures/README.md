# CNN-Architectures

Here I try to explain various computer vision architectures and implement the same using Tensorflow Keras framework.

### 1. AlexNet
Introduced by Krizhevsky et al. in ImageNet Classification with Deep Convolutional Neural Networks
 
AlexNet is a classic convolutional neural network architecture. It consists of convolutions, max pooling and dense layers as the basic building blocks. Grouped convolutions are used in order to fit the model across two GPUs.

### 2. GoogLeNet
Introduced by Szegedy et al. in Going Deeper with Convolutions
 
GoogLeNet is a type of convolutional neural network based on the Inception architecture. It utilises Inception modules, which allow the network to choose between multiple convolutional filter sizes in each block. An Inception network stacks these modules on top of each other, with occasional max-pooling layers with stride 2 to halve the resolution of the grid.
