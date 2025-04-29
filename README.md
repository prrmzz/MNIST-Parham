# MNIST Handwritten Digit Classification with CNN

This project implements a Convolutional Neural Network (CNN) using TensorFlow and TensorFlow Datasets to classify handwritten digits from the MNIST dataset.

## Overview

**Dataset**: MNIST (60,000 training and 10,000 test grayscale images of size 28×28)  
**Framework**: TensorFlow 2.x  

**Model Architecture**:
- Convolutional + BatchNorm + ReLU (×2)  
- MaxPooling + Dropout  
- Convolutional + BatchNorm + ReLU (×2)  
- MaxPooling + Dropout  
- Fully connected layers with Dropout  
- Softmax output (10 classes)

## Preprocessing

- Normalization: Pixel values scaled to [0, 1]  
- Batched, cached, shuffled, and prefetched for performance

## Training

- **Loss**: Sparse Categorical Crossentropy  
- **Optimizer**: Adam  
- **Epochs**: 10  
- **Batch Size**: 256  

## Results

- **Final Test Accuracy**: **99.44%**  
- Accuracy and loss curves are plotted for both training and validation sets.
