# Assignment 03 — Forward Propagation, Backpropagation, and Learning Rate Analysis

## Overview

This assignment focuses on understanding how a neural network learns through **forward propagation and backpropagation** using TensorFlow/Keras. It also investigates how different **learning rates** and **numbers of training epochs** affect the performance of a neural network.

The objective is to understand the training process beyond simply building a model: how inputs move through the network, how predictions are produced, how errors are propagated backwards, and how the model's weights are updated during training.

---

## 1. Forward Propagation

Forward propagation is the process through which input data passes sequentially through the layers of a neural network to produce an output.

Each neuron performs a weighted sum of its inputs, adds a bias, and applies an activation function. The output of one layer becomes the input to the next layer.

The general flow is:

```text
Input Data
    ↓
Layer 1
    ↓
Layer 2
    ↓
Output Layer
    ↓
Prediction
```

The final prediction is then compared with the actual target value to determine the model's error.

---

## 2. Backpropagation

Backpropagation is the process used to update the weights of a neural network based on the error produced by the model.

After forward propagation generates a prediction, a loss function measures the difference between the predicted output and the actual output. Backpropagation calculates how much each model parameter contributed to this error by computing gradients.

An optimizer then uses these gradients to update the model's weights and biases so that the loss can be reduced during subsequent iterations.

The overall learning process can be represented as:

```text
Input
  ↓
Forward Propagation
  ↓
Prediction
  ↓
Loss Calculation
  ↓
Backpropagation
  ↓
Gradient Calculation
  ↓
Weight Update
  ↓
Repeat
```

This process is repeated during training until the model learns useful patterns from the data.

---

## 3. Learning Rate

The **learning rate** controls the size of the updates made to the model's parameters during optimization.

A very small learning rate can make training slow because the model takes small steps toward the optimum. A very large learning rate can cause the training process to become unstable or overshoot a good solution.

The assignment experiments with different learning rates to observe their effect on model training and final performance.

In general:

```text
Small Learning Rate
→ Smaller updates
→ Potentially slower convergence

Large Learning Rate
→ Larger updates
→ Faster but potentially unstable training
```

Comparing different learning rates helps identify how the choice of optimizer settings influences the learning behaviour of the model.

---

## 4. Number of Epochs

An **epoch** represents one complete pass through the training dataset.

The assignment also examines how changing the number of epochs affects model performance. Training for too few epochs may result in underfitting because the model has not had enough opportunities to learn from the data. Training for more epochs can improve performance up to a point, although excessive training may lead to overfitting depending on the dataset and model.

The experiments therefore compare model behaviour across different numbers of training epochs.

---

## 5. Performance Analysis

The results from different learning-rate and epoch configurations are compared to understand their impact on the model.

The analysis considers factors such as:

- Training performance.
- Model convergence.
- Final accuracy or other relevant performance metrics.
- Effect of increasing or decreasing the learning rate.
- Effect of training for fewer or more epochs.

This provides practical insight into why hyperparameter selection is important when training neural networks.

---

## 6. Concepts Covered

This assignment demonstrates the fundamental neural-network training workflow:

```text
Input Data
   ↓
Forward Propagation
   ↓
Prediction
   ↓
Loss
   ↓
Backpropagation
   ↓
Gradient Descent / Optimization
   ↓
Updated Weights
   ↓
Next Epoch
```

It also demonstrates how training hyperparameters, particularly the **learning rate** and **number of epochs**, influence the performance and convergence of a neural network.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Google Colab

## Google Colab

[Open Assignment 03 in Google Colab](https://colab.research.google.com/drive/1Lcie7EWBlF3BefZPXI3jStklNp8ucpb6?usp=sharing)

## Files

- `DL_L3.ipynb` — Complete implementation and experimental analysis for Assignment 03.
