# Implementation-of-VGG-11-architecture
Implementing VGG 11 like architecture on CIFAR 10 dataset

 # Introduction to VGG Architecture
 The VGG architecture is a deep convolutional neural network that comprises of 3x3 stacked convolutional kernel in all its layers.
 The VGG tackles a problem of increasing the depth of our convolutional networks and its effect on its perfomance when dealing with large scale image tasks.

 # Architecture of the VGG network
 The VGG has different configurations ranging from VGG 11 to VGG 16 (11/16 represents the number of weights layers), The VGG network takes 224x224 RGB image as an input, uses a  3x3conv kernel  with stride 1 and padding of 1 and applies a 2x2 max-pooling with  stride of 2 and ends with three fully connected layers with the first two containing 4096 neurons and the Final F layer containing 1000 neurons for ImageNet classification.

 # Experiment
 In this project a VGG 11 like network was implemented and trained on CIFAR 10 dataset which consists of  10 classes (Original was trained on Image net with a 1000 classes), Due to the modification of the final classification layer and the images dimension the model has a total parameter count of 2.8million instead of the  133 million parameters that was reported in the original paper.

 I experienced experienced slow training due to VGG'S large parameters count and due to the architecture originally  designed for ImageNet dataset instead of CIFAR 10 datasets.

To help curb this problem reducig the two Fully connected layers dimensionality would reduce the total parameter count of the architecture and might reduce training cost
 
 

