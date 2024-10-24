# Deep Learning Models for Imbalanced Time Series Clinical Dataset

This repository contains experiments and implementations of various Deep Learning models aimed at improving performance on imbalanced time-series clinical data. The project explores data augmentation techniques and model optimization to enhance classification results in challenging imbalanced datasets.

## Project Overview

The primary goal of this project is to apply and experiment with different deep learning methods to handle imbalanced time-series clinical data. Several techniques, including data augmentation with SMOTE, model optimization, and feature selection, were employed to maximize performance metrics such as AUC.

### Key Features:
- **10 Deep Learning Methods**: Experimentation with models like RNN (with Echo State Network), Transformer, and others.
- **Imbalanced Data Handling**: Utilized **SMOTE** and **Borderline SMOTE** to address class imbalance (49% imbalance).
- **Feature Selection**: Employed Random Forest Feature Ranking to identify key features in the dataset.
- **Performance Metrics**: Achieved a maximum AUC score of **0.95** through careful model tuning.

## Methods and Techniques

1. **Data Augmentation:**
   - **SMOTE (Synthetic Minority Over-sampling Technique)**: Generated synthetic samples for the minority class.
   - **Borderline SMOTE**: A more advanced version of SMOTE that focuses on difficult-to-classify data points near the decision boundary.

2. **Deep Learning Models Tested:**
   - **RNN with Echo State Networks (ESN)**: A variant of recurrent neural networks that simplifies training by using a reservoir of randomly connected neurons.
   - **Transformer**: Applied transformer-based models to capture complex patterns in the time-series data.
   - **Random Forest Feature Ranking**: Used to reduce dimensionality and focus on the most important features in the dataset.

3. **Model Tuning and Optimization:**
   - Performed **hyperparameter tuning** to optimize the deep learning models using techniques such as grid search and random search.
   - Used **TensorFlow** for model implementation and training.

## Results

- **Max AUC:** 0.95 achieved after applying data balancing techniques and optimizing the deep learning models.
- **Improvement in Time-Series Performance:** Significant improvement in classification accuracy, recall, and F1-score due to the use of SMOTE and advanced deep learning architectures.

## Requirements

- **Python 3.x**
- **TensorFlow**: `pip install tensorflow`
- **scikit-learn**: `pip install scikit-learn`
- **imbalanced-learn**: `pip install imbalanced-learn` (for SMOTE and Borderline SMOTE)
- **numpy**, **pandas**, **matplotlib**

