# GAN-Implementation

## Description
This repository contains my approach for implementing generative adversarial networks. I have performed various steps in for implementation including data gathering, data preprocessing,building and training model , evaluating model .

## About the dataset
The CAT dataset includes over 9,000 cat images. For each image, there are annotations of the head of cat with nine points, two for eyes, one for mouth, and six for ears but the GANs are unsupervised learning algorithm hence I do not need the annotations, only cat images are required.

## Data Preprocessing

The Preprocessing method which I have performed is Data Augmentation. Data Augmentation is a
method of artificially increasing the dataset by creating modified copies of the dataset with the help
existing data.
I have chosen Data Augmentation because produces various images from existing images by performing the followings :-
- Rotation 
- Width shift 
- Height shift 
- Zoom 
- Horizontal flip
Data Augmentation also increases the size of dataset which helps in training the Neural Network better
and avoids overfitting.

## Model Building

I have taken around 5000-600 images of cat for model so my model has 7 deconvolutional layers in the generator ,6 convolution layers in the discriminator. After each deconvolutional and convolution layers I have applied Batch normalization and used leaky relu activation function in all the layers of generator and discriminator except the last one in which I have put sigmoid as the activation function. Along with these I have added padding and strides as well.

## Model Training

I had put the model on training on over 5000-6000 cat images with 5500 epochs.

### GAN LOSS 
Check [GAN Loss](https://github.com/redeagle17/GAN-Implementation/tree/main/GAN%20loss).

### Images generated from GAN
Check [Image](https://github.com/redeagle17/GAN-Implementation/tree/main/Generated%20Images).

## Limitations and Improvement

### Limitations
- I didn't train model on entire training dataset.
- Various other data preprocessing technique can be applied.
- The training ran till 3803 epochs for over 11 hours and then stopped abruptly. 

### Improvements
- More complex model design can be used.
- increasing total number of epochs and size of dataset.





