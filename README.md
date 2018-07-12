# Convolutional Neural Network (CNN):

This type of network is really famous in image processing. As a matter of fact most of the nets introduced during the imageNet competition are use convolution operations.

## How does it works ?

When we use a simple neural network like a perceptron or multi layer perceptron and we feed it the image it learns features about it. Here the principle stay the same. The only thing is that we add convolutionnal layers which work like filters. It's like creating a lot of different variations of the image using multiple filters. This allow to get more abstract features and be able to classify more easily.

But to make the model really efficient and avoid overfitting the training data CNNs also use Max Pooling operations. This step reduce a pixel region into 1 "bigger" pixel by keeping the maximum value of all the pixel of that region or the average. This allow easier computation and it also get rid of some noise by making the pattern less specific (group of pixel instead of all of them == more global pattern).

## How to get better ?

Some changes about learning rate, training iterations, optimizer, dropout, adding decay, adding layers, modify operations' parameters could improve the model. But it could also increase significantly the training time and cost more in computation power. Everything is about balance the model needs to be efficient but it shouldn't be too slow or too demanding in computation power otherwise no one will use it.

Inception and VGGNet and others famous CNNS trained on thousands of class are introduced in this link so check it out : 
https://medium.com/@sidereal/cnns-architectures-lenet-alexnet-vgg-googlenet-resnet-and-more-666091488df5

Explanations of the code are inside the notebook. 

For this exemple we used tensorflow to calssify the MNIST dataset.
