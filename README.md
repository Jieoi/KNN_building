# Machine Learning Project: kNN Implementation and Cross-Validation

## Overview

This repository contains the implementation of the k-Nearest Neighbors (kNN) algorithm and cross-validation techniques as part of the coursework for the University of London (UoL) BSc Computer Science project on machine learning.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
    - [Visualizing the Data](#visualizing-the-data)
    - [Exploratory Data Analysis under Noise](#exploratory-data-analysis-under-noise)
      - Q1. Exploratory Data Analysis
      - Q2. Data with Noise
      - Q3. Classifier Evaluation
      - Q4. Nested Cross-validation
- [Requirements](#requirements)

## Introduction

The primary goal of this project is to implement the kNN algorithm and explore its performance through cross-validation. The kNN algorithm is a simple yet effective machine learning algorithm used for classification and regression tasks. Cross-validation is employed to evaluate the model's robustness and generalization capabilities.

## Features

### Wine Classification with k-Nearest Neighbors (kNN) and Cross-validation

### Exploratory Data Analysis

This project focuses on the Wine dataset, consisting of 178 samples categorizing three different types of Italian wine with 13 features. The selected features include 'alcohol,' 'flavanoids,' 'color_intensity,' and 'ash.'

#### Visualizing the Data

A custom function, `myplotGrid`, is provided for visualizing feature interactions through scatter plots and histograms. An alternative Seaborn implementation is included for comparison.

#### Exploratory Data Analysis under Noise

Gaussian noise is introduced to observe its impact on the dataset, and visualizations are generated to compare noisy and clean data.

**Q1. Exploratory Data Analysis**

Based on the analysis, 'flavanoids' and 'color intensity' are selected as the key features for the classifier due to their positive correlation and distinct separation for different wine classes.

**Q2. Data with Noise**

The comparison indicates that while the overall trend remains similar, noise increases the spread of data points, making patterns less clear.

#### Implementing kNN

A k-Nearest Neighbors (kNN) classifier is implemented using basic numpy and matplotlib functions. Helper functions include distance calculation and train-test split.

**Q3. Classifier Evaluation**

Custom functions are created for confusion matrix, accuracy, precision, and recall calculations. Evaluation metrics are printed for the kNN algorithm's output, with results compared to scikit-learn's implementation for verification.

**Q4. Nested Cross-validation**

A nested 5-fold cross-validation is implemented for both original and noisy datasets, considering various k values and distance functions. The evaluation includes accuracy on the validation set, the best parameters, and the confusion matrix for each fold on the testing set.

## Requirements

Ensure you have the following dependencies installed:

- Python (version >= 3.6)
- NumPy
- Scikit-learn
- Matplotlib (for visualization)
