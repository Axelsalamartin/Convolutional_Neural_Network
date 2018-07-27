# Convolutional Neural Network (CNN):

This type of network is really famous in image processing. As a matter of fact most of the nets introduced during the imageNet competition use convolution operations.

## How does it works ?

When we use a simple neural network like a perceptron or a multi layer perceptron and we feed it images, it learns features about it. Here the principle stay the same. The only thing is that we add convolutionnal layers which work like filters. It's like creating a lot of different variations of the images using multiple filters. This allows to get more abstract features and be able to classify more easily.

But to make models really efficient and avoid overfitting CNNs also use Max Pooling operations. This step reduce a pixel region into 1 "bigger" pixel (by keeping the maximum value of all the pixels of that region or the average). This allows easier computation and it also gets rid of some noise by making the patterns less specific (group of pixels instead of all of them == more global patterns).

## How to get better ?

Some changes on : learning rate, training iterations, optimizer, dropout, adding decay, adding layers, modify operations' parameters could improve the model. But it could also increase significantly the training time and cost more in computation power. Everything is about balance the model needs to be efficient but it shouldn't be too slow or too demanding in computation power otherwise no one will use it.

Inception, VGGNet and others famous CNNS trained on thousands of classes are introduced in this link so check it out : 
https://medium.com/@sidereal/cnns-architectures-lenet-alexnet-vgg-googlenet-resnet-and-more-666091488df5

Explanations of the code are inside the notebook. 

For this exemple we use tensorflow to calssify the MNIST dataset.
