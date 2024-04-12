# CIFAR-10 Image Classification

This repository contains code for training an advanced neural network model to classify images from the CIFAR-10 dataset. The model architecture is designed to achieve high accuracy on this classification task, using techniques such as adaptive pooling, dropout, and leaky ReLU activations.

## Table of Contents
1. Introduction
2. Model Architecture
3. Training and Evaluation
4. Results

## Introduction
In this project, we aim to build a powerful neural network model capable of accurately classifying images from the CIFAR-10 dataset. The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. The goal is to correctly identify the object present in each image.


## Model Architecture

Network Architecture
![Architecture](https://github.com/amannaredi/ECS7026P_CIFAR_Dataset_Classification/assets/81749870/e563e089-78ba-465f-84f3-0644e934fe35)

Intermediate Block Architecture
<img width="891" alt="block architecture" src="https://github.com/amannaredi/ECS7026P_CIFAR_Dataset_Classification/assets/81749870/698929b5-d153-467b-9f41-93ff52501141">

Output Block Architecture
<img width="865" alt="Output Block" src="https://github.com/amannaredi/ECS7026P_CIFAR_Dataset_Classification/assets/81749870/b79ceeae-34a6-47c5-983d-457fc311a66d">


The neural network uses a series of intermediate blocks followed by an output block as described below:

- **Intermediate Blocks (B1, B2, ..., BK):** Each block processes the input image through multiple independent convolutional layers, combining their outputs based on a dynamically computed coefficient vector.
- **Output Block (O):** This block processes the output from the last intermediate block to produce the final class logits using fully connected layers.
The neural network model consists of several intermediate blocks, each containing multiple convolutional layers with adaptive pooling, dropout, and leaky ReLU activations. The output block processes the final features to produce logits for classification.

## Training and Evaluation
The model is trained using the CIFAR-10 training dataset and evaluated using the test dataset. We utilize cross-entropy loss as the loss function and Adam optimizer for training. Training progresses over a fixed number of epochs, with periodic evaluation on the test dataset to monitor performance.

## Results
After training the model, we achieved a peak accuracy of 90.06% on the test dataset. The training process and performance metrics are visualized in the provided plots.


Details of the architecture are illustrated in the notebook.
