# Assignment 02 — Multilayer Perceptron for Classification

## Overview

This assignment focuses on designing and implementing a **Multilayer Perceptron (MLP)** for a classification problem using the **Iris or Wine dataset**. The goal is to understand how a basic feed-forward neural network can learn patterns from labelled data and classify samples into their respective categories.

An MLP is an artificial neural network made up of an input layer, one or more hidden layers, and an output layer. Each neuron applies a weighted transformation followed by an activation function, allowing the network to learn non-linear relationships in the input data.

---

## 1. Dataset

The assignment uses a standard classification dataset such as the **Iris dataset**, where each sample is described by numerical features and belongs to one of several classes.

The dataset is divided into input features (`X`) and target labels (`y`). The features are used by the neural network to learn the characteristics of each class.

---

## 2. Data Preparation

Before training the MLP, the dataset is prepared for use by the neural network. The data is split into training and testing sets so that the model can be trained on one portion of the data and evaluated on previously unseen samples.

Feature scaling/normalization is applied where required so that the input features are on suitable numerical scales for neural-network training.

---

## 3. Multilayer Perceptron (MLP)

The MLP is implemented as a feed-forward neural network. Information flows from the input layer through the hidden layer(s) to the output layer.

The hidden layers allow the network to learn increasingly useful representations of the input features. During training, the model adjusts its weights and biases to reduce the classification error.

The general structure can be represented as:

```text
Input Features
      ↓
Hidden Layer(s)
      ↓
Output Layer
      ↓
Predicted Class
```

For a multi-class classification problem, the output layer produces values corresponding to the possible classes, which are used to determine the predicted class.

---

## 4. Model Training

The MLP is trained using the training portion of the dataset. During training, the network processes the input samples, generates predictions, calculates the classification loss, and updates its parameters using backpropagation and an optimization algorithm.

The training process allows the network to learn the relationship between the input features and their corresponding class labels.

---

## 5. Performance Evaluation

After training, the model is evaluated using the test dataset. Two important evaluation methods are used:

### Accuracy

Accuracy measures the proportion of test samples that are classified correctly.

```text
Accuracy = Correct Predictions / Total Predictions
```

A higher accuracy indicates that the MLP correctly classifies a larger proportion of the unseen test samples.

### Confusion Matrix

A **confusion matrix** provides a more detailed view of classification performance by comparing the actual classes with the classes predicted by the model.

It shows how many samples from each class were:

- Correctly classified.
- Incorrectly classified as another class.

This is particularly useful for identifying which classes the model has difficulty distinguishing.

---

## 6. Concepts Covered

This assignment demonstrates the complete workflow for a basic neural-network classification task:

```text
Dataset
   ↓
Data Preparation
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Build MLP
   ↓
Train Model
   ↓
Generate Predictions
   ↓
Evaluate Accuracy
   ↓
Analyze Confusion Matrix
```

The assignment provides a practical introduction to using a neural network for supervised classification and evaluating its performance on unseen data.

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

## Google Colab

[Open Assignment 02 in Google Colab](https://colab.research.google.com/drive/1EkLvRd2adpYb8WnJ330kVcFRnSt2wqQO?usp=sharing)

## Files

- `DL_L2.ipynb` — Complete implementation of the MLP classification assignment.
