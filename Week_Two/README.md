## Goal
In this notebook, you're going to create another GAN using the MNIST dataset. You will implement a Deep Convolutional GAN (DCGAN), a very successful and influential GAN model developed in 2015.

Note: here is the paper if you are interested! It might look dense now, but soon you'll be able to understand many parts of it :)

## Learning Objectives
Get hands-on experience making a widely used GAN: Deep Convolutional GAN (DCGAN).
Train a powerful generative model.
Generator architecture

Figure: Architectural drawing of a generator from DCGAN from Radford et al (2016).

## Getting Started
DCGAN
Here are the main features of DCGAN (don't worry about memorizing these, you will be guided through the implementation!):

Use convolutions without any pooling layers
Use batchnorm in both the generator and the discriminator
Don't use fully connected hidden layers
Use ReLU activation in the generator for all layers except for the output, which uses a Tanh activation.
Use LeakyReLU activation in the discriminator for all layers except for the output, which does not use an activation
You will begin by importing some useful packages and data that will help you create your GAN. You are also provided a visualizer function to help see the images your GAN will create.
