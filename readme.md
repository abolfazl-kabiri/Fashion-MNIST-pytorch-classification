# Computational Intelligence Project: MLP vs. CNN for Fashion-MNIST Classification

## Project Overview
This project implements and compares two fundamental neural network architectures—a Multilayer Perceptron (MLP) and a Convolutional Neural Network (CNN)—for the task of classifying images from the Fashion-MNIST dataset.

The primary goal is to demonstrate and quantify the superior performance of CNNs in extracting spatial features from image data compared to traditional MLPs, which treat the input as a flattened vector.

## Dataset
The project uses the Fashion-MNIST dataset, which consists of 70,000 grayscale images (60,000 training, 10,000 testing) of clothing items across 10 classes (e.g., T-shirt, Trouser, Sneaker, Ankle boot). Each image is 28x28 pixels.

## Models Implemented
### MLP
- File: MLP.ipynb
- Architecture: Linear(784, 256) -> Linear(256, 128) -> Linear(128, 64) -> Linear(64, 32) -> Linear(32, 10)

### CNN
- File: CNN.ipynb
- Architecture: Conv(1, 32) -> MaxPool -> Conv(32, 64) -> MaxPool -> Flatten -> Linear(3136, 128) -> Linear(128, 10)
