# Optimizing SVM Classifier with UCIML Dataset

This repository hosts code for optimizing an SVM (Support Vector Machine) classifier using random values and iterations on a dataset obtained from the UCIML repository.

## Introduction
Support Vector Machines (SVMs) are potent supervised learning models utilized for classification tasks. They function by identifying the optimal hyperplane that effectively separates classes in a high-dimensional space. Optimizing SVM parameters, including kernel type, regularization parameter (C), and kernel coefficient (gamma), is pivotal for achieving optimal performance.

## Dataset
The dataset utilized in this project is sourced from the UCIML repository. It furnishes details on various features of dry beans, aiming to categorize them into distinct classes based on these features. The dataset encompasses features like area, perimeter, compactness, length, width, asymmetry coefficient, and length of kernel groove. For the classification model, images of 13,611 grains of 7 different registered dry beans were captured with a high-resolution camera. These bean images, obtained via a computer vision system, underwent segmentation and feature extraction stages, yielding a total of 16 features; 12 dimensions and 4 shape forms, extracted from the grains.

Dataset Snapshot:
![](https://github.com/kunalarora0930/Parameter-Optimization-of-SVM-Assignment/blob/main/Dry_bean.png)

## Code Overview
The primary code file, `svm_classifier_optimization.py`, encompasses the implementation of SVM classifier optimization using random values and iterations. Here's a concise overview of the code:
- **Data Loading**: The dataset is fetched from the UCIML repository using the `fetch_ucirepo` function provided by the `ucimlrepo` library. Subsequently, the dataset is loaded into pandas DataFrames.
- **Data Preprocessing**: While the provided code snippet doesn't explicitly showcase preprocessing steps, procedures such as data cleaning, feature scaling, or encoding categorical variables can be applied based on the dataset's requisites.
- **SVM Classifier Optimization**:
  - Random values for SVM parameters (kernel type, C, gamma) are generated.
  - SVM classifier is trained using these random parameters.
  - Performance metrics (accuracy) are evaluated.
  - The process iterates for a specified number of iterations.
- **Results Visualization**: The achieved best accuracy during optimization is exhibited, along with an analysis table illustrating the best parameters and a convergence plot demonstrating accuracy over iterations.

## Dependencies
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `ucimlrepo`

## Results
The following Analysis Table and Convergence Graph were generated for this project. The Convergence Graph represents the sample with the overall best accuracy.

Analysis Table:
![](https://github.com/kunalarora0930/Parameter-Optimization-of-SVM-Assignment/blob/main/Analysis_table.png)

Convergence Graph:
![](https://github.com/kunalarora0930/Parameter-Optimization-of-SVM-Assignment/blob/main/Convergence_Graph.png)

