# DefenseAgainstAdverserialInput
Study of Adversarial Attack and Defense Methods

## Introduction

Neural network is vulnerable to adversarial examples, which means that inputs formed by adding small perturbations will make network output incorrect answer with high confidence. Hence, it isdifficult to apply neural networks in security-critical areas. Our

## Our Basic Setup

Dataset: Digit-recognition task (0-9) standard dataset MNIST
Network Structure: shown on the right
Our defense method focuses on the CW attack algorithm

![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/4.png)

## The Original Result

The accuracy of the neural network is 99% for the original data.
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/1.png)

## State-of-the-art attack algorithms: 
## FGSM Algorithm & C&W Algorithm

FGSM: We find that this method reliably causes a wide variety of models to misclassify their input by causing a small  shift in the values of the input.
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/2.png)

C&W: Dataset: Digit-recognition task (0-9) standard dataset MNIST
Measure of modification: Throughout our project, we have used the L2 distance. It measures the standard Euclidean (root mean-square) distance between x and x’ .
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/3.png)

Motivation for L2:
The L2 norm is more stable than the L1 norm, although more rigorous to compute. L2 has just one solution compared to L1 which has multiple

## For FGSM, the accuracy is 29.8%, and images generated are as follows:
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/5.png)

## For CW, the accuracy is 22.5%, and images generated are as follows:
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/6.png)

# Part 1 results: JPEG Compression
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/7.png)

# Part 2 introduction: Low Pass Filter
Gaussian filter: modify the input image by convolution with a Gaussian function, used to reduce image noise and reduce detail
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/8.png)

## Part 2 results : Low Pass Filter
The accuracy for examples filtered by low pass filter is 99% when sigma = 1
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/9.png)

# Part 3: JPEG Compression & Resolution Enhancement 
Resolution Enhancement is a method to make the image look CLEARER
We used pretrained neural network(vgg19 etc.)

Why we use it:
Compression eliminates some noise, while makes the image blurry
Enhancing the resolution repairs the important portions of the image and helps increases accuracy.

![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/10.png)

# Summary of project
![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/11.png)

![cnn](https://github.com/nikki30/Defense-Against-Adverserial-Input/blob/master/img/7.png)
  
