# Kidney Cancer Detection: Binary Classification (Normal vs. Tumor)

A specialized Deep Learning implementation using Convolutional Neural Networks (CNN) to distinguish between healthy kidney scans and those containing tumors.

## 🚀 Overview

This specific project focus is on the binary classification of kidney medical images. It provides a highly accurate model for identifying the presence of cancer, which serves as the first step in automated medical diagnosis.

## ✨ Key Features

- **High Accuracy**: Achieves a test accuracy of **99.95%** on histological images.
- **Automated Data Pipeline**: Uses `gdown` to fetch data and `rarfile` for seamless extraction.
- **Structured CNN**: A 5-layer convolutional design optimized for binary feature extraction.
- **Dataset Splitting**: Predefined 80/20 train-test split handling via directory flow.

## 📊 Dataset Detail

The dataset classifies images into two categories:

1.  **kidney_normal**: Images of healthy kidney tissue.
2.  **kidney_tumor**: Images featuring confirmed tumor tissue.

## 🏗️ Model Architecture

The architecture is built for binary discrimination:

- **Input**: 224x224 RGB images.
- **Backbone**: 5 Conv2D layers (filters: 32, 64, 128, 256, 512) with ReLU activation.
- **Head**: Dropout/Dense layers followed by a 2-node Softmax output.
- **Optimization**: Adam optimizer with Categorical Cross-Entropy loss.

## 🛠️ How to Run

1.  Open `kidney cancer detection1.ipynb` in your environment.
2.  Set up your Google Drive mount if running in Colab.
3.  Execute all cells to:
    - Download the `Kidney_Cancer_Dataset.rar`.
    - Extract to the `/content` directory.
    - Visualize training metrics.
    - Verify test results.

## 📈 Performance Summary

- **Final Test Accuracy**: 99.95%
- **Final Test Loss**: 0.0049
- **Training Epochs**: 10

## 💻 Tech Stack

- Python 3.x
- TensorFlow 2.x
- Keras
- Matplotlib (Plotting)
- Gdown (Networking)
- Rarfile (Archive handling)
