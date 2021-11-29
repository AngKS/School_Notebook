# AlexNet; the Architecture that challenged CNNs

<div align='center'>
<img src='https://github.com/AngKS/School_Notebook/blob/master/ST1504_Deep_Learning/assets/brain.jpeg?raw=true' width='400' height='300' />
</div>



## The Problem
Convolutional Neural Networks(CNNs) have always been the goto model for object recognition and image classification. They are stronger, easy to control and even easier to train. They don't experience any overfitting at any alarming scales while being used on millions of images. Their performance is almost identical to tandard feed-forward neural networks of the same size.

However, they are extremely difficult to apply to high resolution images.

## Architecture of AlexNet
![Model Architecture](https://github.com/AngKS/School_Notebook/blob/master/ST1504_Deep_Learning/assets/architecture.png?raw=true)

The architecture consists of 8 layers; 5 convolutional layers, 2 fully-connected layers and a softmax layer.
This alone does not make AlexNet anything special... that is until we add in some features and new approaches to the convolutional layers:

- **ReLU non-Linearity**

AlexNet uses Rectififed Linear Units(ReLU) instead of the tanh non-linearity that is used which was standard at that time. ReLU's advantage lies in its training time. A CNN using ReLU was able to reach 25% error on CIFAR-10 dataset 6 times faster thana CNN using tanh.

- **Multiple GPUs**

AlexNet allows for multi-GPU training by putting half its neurons on one GPU and the other half on another GPU. Not only does this mean that a bigger model can be trained; the time taken to train the model will also cut down.

- **Overlapping Layers**

CNNs traditionally "pool" outputs of neighboring groups of neurons with no overlapping. However, when overlap was introduced, the model saw a reduction in error by about 0.5% and models with oveerlapping pooling generally find it harder to overfit.

### The Overfitting Problem

AlexNet had 60 million of parameters, a major issue in terms of **Overfitting**. 2 methods were employed to combat this problem:

1. **Data Augmentation**

The model uses label-preserving transformation to make the data more varied. Specifically, the makers generated image translatiopns and horizontal reflections that increasd the trianing set by a factor of 2048. They also performed Principal Component Analysis(PCA) on the RGB pixel values to change the intensities of the RGB channels which reduced the top-1 error rate by more than 1%.

2. **Dropout**

