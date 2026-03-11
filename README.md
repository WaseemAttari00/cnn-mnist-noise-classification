# CNN for Handwritten Digit Classification with Correlated Noise

## Overview

This project implements a **Convolutional Neural Network (CNN)** to classify handwritten digits from a modified **MNIST dataset containing correlated noise**.

The goal is to evaluate how well a deep learning model can correctly recognize handwritten digits even when the images are corrupted with structured noise.

The project demonstrates a complete **deep learning workflow**, including:

* Data preprocessing
* CNN architecture design
* Model training and validation
* Model evaluation

---

## Dataset

The dataset used is a modified version of the **MNIST handwritten digits dataset**, where images contain **correlated noise**.

Each sample includes:

* A **28 × 28 grayscale image**
* A **digit label (0–9)**

The dataset is stored as:

MNIST_CorrNoise.npz

---

## Technologies Used

* Python
* NumPy
* TensorFlow / Keras
* Matplotlib
* Jupyter Notebook

---

## Model Architecture

The model is a **Convolutional Neural Network (CNN)** consisting of:

* Convolutional layers for feature extraction
* MaxPooling layers for spatial down-sampling
* Fully connected (dense) layers for classification
* Softmax output layer for multi-class prediction

Loss Function:
categorical_crossentropy

Optimizer:
Adam / SGD

---

## Training Configuration

| Parameter        | Value |
| ---------------- | ----- |
| Batch Size       | 128   |
| Epochs           | 45    |
| Validation Split | 20%   |

Training callbacks used:

* EarlyStopping
* ModelCheckpoint
* ReduceLROnPlateau

These techniques help prevent **overfitting** and improve training stability.

---

## Results

The CNN successfully learns to classify handwritten digits even when the images contain correlated noise.

The convolutional layers extract spatial features that allow the model to maintain strong classification performance despite noisy inputs.

---
