# Dog vs. Cat Classification using CNN

This repository contains a Computer Vision pipeline implemented in Python using **TensorFlow/Keras**. The project uses a Convolutional Neural Network (CNN) to classify images as either a **dog** or a **cat**.

## 📌 Project Overview
The pipeline handles the entire machine learning workflow, including:
- Data loading and preprocessing (image normalization and reshaping).
- Visualization of the dataset.
- Building a Sequential CNN architecture.
- Training the model with binary cross-entropy loss.
- Evaluating performance on a separate test set.
- Making predictions on individual random samples.

## 🛠️ Technical Stack
- **Language:** Python 3.x
- **Deep Learning Framework:** TensorFlow / Keras
- **Numerical Processing:** NumPy
- **Visualization:** Matplotlib

## 🏗️ Model Architecture
The model is built using a `Sequential` stack of layers:
1. **Conv2D Layer:** 32 filters, (3,3) kernel, ReLU activation (Input: 100x100x3).
2. **MaxPooling2D:** (2,2) pool size.
3. **Conv2D Layer:** 32 filters, (3,3) kernel, ReLU activation.
4. **MaxPooling2D:** (2,2) pool size.
5. **Flatten Layer:** To convert 2D features to a 1D vector.
6. **Dense Layer:** 64 units, ReLU activation.
7. **Dense Layer (Output):** 1 unit, Sigmoid activation (for binary classification).

## 📂 Dataset Structure
To run the notebook, your project structure should look like this:
```text
├── dataset/
│   ├── input.csv         # Training images (flattened)
│   ├── labels.csv        # Training labels (0 for dog, 1 for cat)
│   ├── input_test.csv    # Test images
│   └── labels_test.csv   # Test labels
├── cvdpipeline.ipynb     # Main Jupyter Notebook
└── README.md
