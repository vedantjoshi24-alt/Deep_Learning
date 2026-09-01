# Assignment 01 — Data Preprocessing and Visualization using TensorFlow/Keras

## Overview

This assignment introduces the basic workflow used when working with datasets for Deep Learning models. The implementation is performed using **TensorFlow and Keras in Google Colab**.

The assignment uses the **MNIST handwritten digit dataset**, which contains grayscale images of handwritten digits from 0 to 9. Each image is represented as a 28 × 28 matrix of pixel values ranging from 0 to 255.

The main purpose of this assignment is to understand how raw data is loaded, explored, preprocessed, normalized, divided into training and testing sets, and visualized before it is provided to a Deep Learning model.

---

## 1. TensorFlow and Keras Setup

The assignment begins by importing the required libraries:

- **TensorFlow** — used as the primary Deep Learning framework.
- **Keras** — used for accessing datasets and building Deep Learning models.
- **Matplotlib** — used for visualizing the image data.

The notebook is executed in **Google Colab**, which provides a Python environment with TensorFlow and other required libraries available.

---

## 2. Loading the Dataset

The MNIST dataset is loaded using the Keras dataset API.

The dataset is automatically divided into two parts:

- **Training set** — used to train a machine learning model.
- **Testing set** — used to evaluate the model on data that was not used during training.

Each image in the dataset represents one handwritten digit from 0 to 9.

The images have a resolution of:

```text
28 × 28 pixels
```

Since the images are grayscale, every pixel contains a value between:

```text
0 and 255
```

where 0 represents black and 255 represents white.

---

## 3. Exploring the Dataset

Before preprocessing, the dimensions and contents of the dataset are inspected.

The notebook checks the shape of the training and testing images and also examines the corresponding labels.

This helps in understanding:

- Number of training samples
- Number of testing samples
- Image dimensions
- Structure of the labels

Understanding the shape of the input data is important before feeding it into a Deep Learning model.

---

## 4. Data Normalization

The original pixel values range from 0 to 255.

For Deep Learning, it is generally beneficial to scale these values to a smaller range. In this assignment, the pixel values are normalized by dividing every pixel by `255.0`.

Therefore:

```text
Original range:   0 – 255
Normalized range: 0 – 1
```

For example:

```text
0     → 0.0
128   → 0.502
255   → 1.0
```

Normalization makes the input values easier for a neural network to process and can help improve the stability and efficiency of model training.

---

## 5. Train-Test Split

The MNIST dataset is already provided with separate training and testing sets.

The training data is used for learning patterns from the images, while the testing data is kept separate so that a future model can be evaluated on unseen examples.

This separation helps measure how well a trained model generalizes to new data.

---

## 6. Data Visualization

The assignment uses **Matplotlib** to visualize samples from the dataset.

The images are displayed as grayscale images using `plt.imshow()`.

Visualizing the data is an important preprocessing step because it allows us to verify that:

- The images have been loaded correctly.
- The pixel values represent the expected images.
- The labels correspond to the displayed handwritten digits.
- The dataset has the expected structure.

---

## 7. Concepts Covered

This assignment demonstrates the fundamental data preparation pipeline used in Deep Learning:

```text
Dataset
   ↓
Load Data
   ↓
Explore Dataset
   ↓
Train-Test Split
   ↓
Normalize Data
   ↓
Visualize Data
   ↓
Ready for Deep Learning Model
```

These preprocessing steps form the foundation for subsequent assignments where the processed data can be used to train neural networks.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- Matplotlib
- Google Colab

## Dataset

**MNIST Handwritten Digit Dataset**

The dataset consists of grayscale images of handwritten digits ranging from 0 to 9.

## Google Colab

[Open the Assignment 01 notebook in Google Colab](https://colab.research.google.com/drive/12oLF9dxZbkUX_obR540lt4ZqgAdtTUo2?usp=sharing)

## Files

- `DL_L1.ipynb` — Complete implementation of the assignment.
