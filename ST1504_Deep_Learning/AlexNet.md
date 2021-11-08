# AlexNet; the Architecture that challenged CNNs

<div align='center'>
<img src='https://' width='500' height='500' />
</div>



## The Problem
Convolutional Neural Networks(CNNs) have always been the goto model for object recognition and image classification. They are stronger, easy to control and even easier to train. They don't experience any overfitting at any alarming scales while being used on millions of images. Their performance is almost identical to tandard feed-forward neural networks of the same size.

However, they are extremely difficult to apply to high resolution images.

## Architecture of AlexNet
The architecture consists of 8 layers; 5 convolutional layers, 2 fully-connected layers and a softmax layer.
This alone does not make AlexNet anything special... that is until we add in some features and new approaches to the convolutional layers:

**- ReLU non-Linearity**

AlexNet uses Rectififed Linear Units(ReLU) instead of the tanh non-linearity that is used which was standard at that time. ReLU's advantage lies in its training time,