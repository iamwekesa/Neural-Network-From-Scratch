# Neural-Network-From-Scratch

### Project 01: AI Journey - Decoding Handwritten Digits from First Principles

This repository contains a complete implementation of a **Multi-Layer Perceptron (MLP)** built entirely from scratch using **NumPy**. The project aims to recognize handwritten digits from the MNIST dataset without using high-level deep learning libraries like TensorFlow or PyTorch.

## Overview
The goal of this project was to understand the fundamental mathematics—linear algebra and calculus—that power modern Artificial Intelligence. By building the network from the ground up, we explore how data flows through layers and how a machine learns through error correction.

## Network Architecture
- **Input Layer:** 784 neurons (representing the $28 \times 28$ flattened pixels of an MNIST image).
- **Hidden Layer:** 10 neurons with **ReLU** (Rectified Linear Unit) activation.
- **Output Layer:** 10 neurons (representing digits 0-9) with **Softmax** activation.

## The Pipeline
The project is structured into five core steps:
1.  **Data Preprocessing:** Loading, shuffling, and normalizing MNIST pixel values (0-255) to a scale of 0-1.
2.  **Initialization:** Generating random weights ($W$) and biases ($b$) to break symmetry.
3.  **Forward Propagation:** Computing the linear transformations ($Z = WX + b$) and applying non-linear activation functions.
4.  **Backward Propagation:** Using the chain rule to calculate gradients and determine how much each weight contributed to the prediction error.
5.  **Gradient Descent:** Updating the parameters iteratively to minimize the loss function.

## Results
- **Initial Accuracy:** ~10% (Random guessing)
- **Final Accuracy:** ~85-90% (After 500 iterations)


## Concepts Covered
- Matrix Multiplication (Dot Products)
- One-Hot Encoding
- Derivatives of Activation Functions
- Learning Rates & Hyperparameters