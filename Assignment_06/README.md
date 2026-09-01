# Assignment 06 — Convolutional Neural Network for Image Classification

## Overview

This assignment focuses on designing and implementing a **Convolutional Neural Network (CNN)** for image classification using a plant disease dataset such as the **Tomato or Soybean disease dataset**.

CNNs are a type of Deep Learning architecture particularly suited for image-based tasks. Unlike traditional neural networks, CNNs can automatically learn spatial features such as edges, textures, shapes, and more complex visual patterns directly from images.

The objective of this assignment is to understand how a CNN can process plant images and learn to distinguish between different disease classes.

---

## 1. Dataset

The assignment uses a plant disease image dataset containing images belonging to different disease or health categories.

Each image acts as an input to the CNN, while its corresponding disease category is used as the target label during supervised learning.

Before training, the images need to be prepared into a consistent format and associated with their corresponding class labels.

---

## 2. Image Preprocessing

The raw images are prepared before being passed to the neural network. Typical preprocessing steps include resizing the images to a common input dimension and scaling pixel values to a suitable numerical range.

Preprocessing ensures that the images have a consistent representation and makes the data suitable for efficient CNN training.

The dataset is also divided into training and evaluation portions so that the model can be tested on images that it has not seen during training.

---

## 3. Convolutional Neural Network

The CNN is built using **TensorFlow/Keras**. Its architecture consists of layers that progressively learn visual features from the input images.

A typical CNN workflow is:

```text
Input Image
     ↓
Convolution Layer
     ↓
Activation Function
     ↓
Pooling Layer
     ↓
Convolution Layer
     ↓
Pooling Layer
     ↓
Flatten / Feature Representation
     ↓
Dense Layer(s)
     ↓
Output Layer
     ↓
Predicted Disease Class
```

### Convolution

Convolutional layers apply learnable filters to the input image. These filters detect useful local patterns such as edges, textures, and shapes.

As the network becomes deeper, the learned features can represent increasingly complex structures within the image.

### Pooling

Pooling layers reduce the spatial dimensions of feature maps while retaining important information. This reduces computational requirements and helps the network focus on the most relevant features.

### Dense Layers

After extracting visual features, the resulting representation is passed to dense layers. These layers use the learned features to perform the final classification.

---

## 4. Model Training

The CNN is trained using labelled training images. During training, the model performs forward propagation to generate predictions, calculates the classification loss, and uses backpropagation to update its weights.

Over multiple training epochs, the network gradually learns visual patterns that help distinguish between the different plant disease classes.

---

## 5. Image Classification

After training, the CNN can be given an unseen plant image and produce a prediction for its disease category.

The classification process can be summarized as:

```text
Plant Image
    ↓
Preprocessing
    ↓
Trained CNN
    ↓
Feature Extraction
    ↓
Classification
    ↓
Predicted Disease
```

This demonstrates how CNNs can be applied to real-world agricultural image-classification problems such as identifying plant diseases from leaf images.

---

## 6. Concepts Covered

This assignment provides practical understanding of:

- Convolutional Neural Networks (CNNs)
- Image preprocessing
- Convolutional layers
- Pooling layers
- Feature extraction
- Dense classification layers
- Forward propagation
- Backpropagation
- CNN model training
- Image classification using Deep Learning

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Google Colab

## Google Colab

[Open Assignment 06 in Google Colab](https://colab.research.google.com/drive/1Tgmv_oBldprcW_KjQpUj337IK4NfBBHA?usp=sharing)

## Files

- `DL_L6.ipynb` — Complete implementation of the CNN image-classification assignment.
