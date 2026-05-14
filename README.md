# UE24CS645BC2_PES1PG25CS071_Fashion_MNIST_CNN
Description:
This project implements a Convolutional Neural Network (CNN) from scratch using only NumPy to classify grayscale clothing images from the Fashion MNIST dataset. Unlike typical deep learning projects that rely on high-level frameworks like Keras or PyTorch for model layers, this implementation manually defines the forward and backward passes for each layer, offering a transparent look into the inner workings of a CNN.

What It Does:
Loads and preprocesses the Fashion MNIST dataset (1,000 training images, 200 test images), normalizing pixel values to [0, 1]
Builds a CNN pipeline with three custom layers:

Conv2D — applies 8 learnable 3×3 filters via sliding window convolution
MaxPool2 — performs 2×2 max pooling to downsample feature maps
Softmax — a fully connected output layer with 10 class nodes and softmax activation

Trains the network using stochastic gradient descent with manual backpropagation over 5 epochs
Evaluates the model on test data, reporting loss and accuracy
Visualizes a sample prediction alongside the ground truth label

Architecture:
Input (28×28) → Conv2D (8 filters, 3×3) → MaxPool2 (2×2) → Flatten → Softmax (10 classes)

Classes:
The model classifies images into 10 fashion categories: T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, and Ankle boot.

Key Concepts Demonstrated:
Manual implementation of convolution, max pooling, and softmax layers
Backpropagation through each custom layer
Cross-entropy loss computation
Grayscale image classification

Requirements:
Python 3
NumPy
Matplotlib
TensorFlow / Keras 
