# Banknote Authentication Using Machine Learning

A machine learning and deep learning project for detecting counterfeit banknotes using the **Banknote Authentication dataset** from the UCI Machine Learning Repository.

## Project Overview

The dataset contains **1,372 banknote samples** with four numerical features extracted from high-resolution banknote images using **Wavelet Transform**:

* Variance
* Skewness
* Kurtosis
* Entropy

The target variable is binary:

* `0` — Counterfeit banknote
* `1` — Genuine banknote

The dataset was split into **80% training and 20% testing data**, followed by feature standardization using `StandardScaler`.

## Model Architecture

The final neural network uses:

* Input layer: 4 features
* Dense layer: 16 neurons, ReLU
* Dropout: 20%
* Dense layer: 8 neurons, ReLU
* Dropout: 20%
* Output layer: 1 neuron, Sigmoid
* Optimizer: Adam
* Loss function: Binary Crossentropy
* Early Stopping

## Evaluation

The final model achieved:

* **Test Accuracy:** 100%
* **ROC-AUC:** 1.00
* **Test Loss:** 0.0021

Additional experiments were conducted to compare different optimizers and the effect of Dropout on model performance.

## Technologies

* Python
* TensorFlow / Keras
* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Seaborn

## Dataset

UCI Machine Learning Repository — Banknote Authentication Dataset

https://archive.ics.uci.edu/dataset/267/banknote+authentication
