# Banknote Authentication — Machine Learning Study

A study of banknote classification using the [UCI Banknote Authentication dataset](https://archive.ics.uci.edu/dataset/267/banknote+authentication).

## Repository contents

This repository contains the **[project report](Sahte%20Banknot%20Tespiti%20%28Makine%20Ogrenmesi%29.pdf)**, written in Turkish. Training scripts, notebooks and saved models are not included. The summary below describes the documented experiment.

## Dataset and approach

The dataset contains 1,372 samples with four numerical features derived from banknote images: variance, skewness, kurtosis and entropy. The study uses an 80/20 train/test split and feature standardization with `StandardScaler`.

## Neural network

- Four input features.
- Dense layers with 16 and 8 ReLU units.
- 20% dropout.
- A single sigmoid output.
- Adam optimization, binary cross-entropy and early stopping.

## Reported evaluation

| Metric | Reported value |
| --- | --- |
| Test accuracy | 100% |
| ROC-AUC | 1.00 |
| Test loss | 0.0021 |

These results describe the report's test experiment. They do not establish performance on other datasets or real-world banknotes, and cannot be reproduced from this repository alone.

## Tools used in the study

Python · TensorFlow/Keras · Scikit-learn · Pandas · NumPy · Matplotlib · Seaborn
