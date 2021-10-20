# CNN-Architectures

Here I try to explain various computer vision architectures and implement the same using Tensorflow Keras framework.

### 1. AlexNet
Introduced by Krizhevsky et al. in ImageNet Classification with Deep Convolutional Neural Networks
 
AlexNet is a classic convolutional neural network architecture. It consists of convolutions, max pooling and dense layers as the basic building blocks. Grouped convolutions are used in order to fit the model across two GPUs.

### 2. GoogLeNet
Introduced by Szegedy et al. in Going Deeper with Convolutions
 
GoogLeNet is a type of convolutional neural network based on the Inception architecture. It utilises Inception modules, which allow the network to choose between multiple convolutional filter sizes in each block. An Inception network stacks these modules on top of each other, with occasional max-pooling layers with stride 2 to halve the resolution of the grid.

### 3. VGG
Introduced by Simonyan et al. in Very Deep Convolutional Networks for Large-Scale Image Recognition

VGG is a classical convolutional neural network architecture. It was based on an analysis of how to increase the depth of such networks. The network utilises small 3 x 3 filters. Otherwise the network is characterized by its simplicity: the only other components being pooling layers and a fully connected layer.

### 4. Residual Network
Introduced by He et al. in Deep Residual Learning for Image Recognition
 
Residual Networks, or ResNets, learn residual functions with reference to the layer inputs, instead of learning unreferenced functions. Instead of hoping each few stacked layers directly fit a desired underlying mapping, residual nets let these layers fit a residual mapping. They stack residual blocks ontop of each other to form network: e.g. a ResNet-50 has fifty layers using these blocks.

Formally, denoting the desired underlying mapping as **H(x)**, we let the stacked nonlinear layers fit another mapping of **F(x):= H(x) - x**. The original mapping is recast into **F(x) + x**.
There is empirical evidence that these types of network are easier to optimize, and can gain accuracy from considerably increased depth.

### 5. ResNeXt
Introduced by Xie et al. in Aggregated Residual Transformations for Deep Neural Networks
 
A ResNeXt repeats a building block that aggregates a set of transformations with the same topology. Compared to a ResNet, it exposes a new dimension, cardinality (the size of the set of transformations) **C**, as an essential factor in addition to the dimensions of depth and width.

### 6. Inception-v4, Inception-ResNet and the Impact of Residual Connections on Learning
Introduced by Christian Szegedy, Sergey Ioffe, Vincent Vanhoucke, Alex Alemi

Very deep convolutional networks have been central to the largest advances in image recognition performance in recent years. One example is the Inception architecture that has been shown to achieve very good performance at relatively low computational cost. Recently, the introduction of residual connections in conjunction with a more traditional architecture has yielded state-of-the-art performance in the 2015 ILSVRC challenge; its performance was similar to the latest generation Inception-v3 network. This raises the question of whether there are any benefit in combining the Inception architecture with residual connections. Here we give clear empirical evidence that training with residual connections accelerates the training of Inception networks significantly. There is also some evidence of residual Inception networks outperforming similarly expensive Inception networks without residual connections by a thin margin. We also present several new streamlined architectures for both residual and non-residual Inception networks. These variations improve the single-frame recognition performance on the ILSVRC 2012 classification task significantly. We further demonstrate how proper activation scaling stabilizes the training of very wide residual Inception networks. With an ensemble of three residual and one Inception-v4, we achieve 3.08 percent top-5 error on the test set of the ImageNet classification (CLS) challenge.

