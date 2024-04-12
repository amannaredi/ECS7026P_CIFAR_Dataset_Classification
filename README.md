# CIFAR-10 Image Classification

This project implements a neural network to classify images from the CIFAR-10 dataset using PyTorch. The CIFAR-10 dataset consists of 60000 32x32 color images in 10 different classes. The goal is to develop a model that can accurately classify these images into their respective categories.

## Project Structure
The project is structured as follows:

- `ECS7026P_CIFAR.ipynb`: Jupyter notebook containing the full implementation and execution of the model.


## Model Architecture

![Architecture](https://github.com/amannaredi/ECS7026P_CIFAR_Dataset_Classification/assets/81749870/e563e089-78ba-465f-84f3-0644e934fe35)
<img width="891" alt="block architecture" src="https://github.com/amannaredi/ECS7026P_CIFAR_Dataset_Classification/assets/81749870/698929b5-d153-467b-9f41-93ff52501141">
<img width="865" alt="Output Block" src="https://github.com/amannaredi/ECS7026P_CIFAR_Dataset_Classification/assets/81749870/b79ceeae-34a6-47c5-983d-457fc311a66d">


The neural network uses a series of intermediate blocks followed by an output block as described below:

- **Intermediate Blocks (B1, B2, ..., BK):** Each block processes the input image through multiple independent convolutional layers, combining their outputs based on a dynamically computed coefficient vector.
- **Output Block (O):** This block processes the output from the last intermediate block to produce the final class logits using fully connected layers.

Details of the architecture are illustrated in the notebook.
