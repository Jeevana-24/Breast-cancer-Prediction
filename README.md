# Breast Cancer Prediction

## Abstract
Breast cancer is a major health concern globally, and early detection is key to effective treatment. This project explores the Breast Cancer Wisconsin (Diagnostic) dataset from Kaggle, which includes data from fine needle aspirate (FNA) biopsies. Using various machine learning algorithms, we aim to build a predictive model to classify tumors as either malignant or benign.

## Dataset Overview
The dataset contains 33 columns, including a target diagnosis column. Features include measurements like radius, texture, smoothness, and compactness of the cell nuclei. Unnecessary columns like 'Unnamed' (null values) and 'id' (irrelevant to the output) were removed. The 'diagnosis' column was encoded from categorical ('M' for malignant and 'B' for benign) to numerical values (1 and 0, respectively).

## Preprocessing
- Removed 'Unnamed' and 'id' columns.
- Transformed 'diagnosis' from categorical to numerical.
- Scaled and encoded other relevant features for model training.

## Machine Learning Models Used

- **Spectral Clustering**

## Spectral Clustering
Spectral clustering is utilized due to its effectiveness with high-dimensional data and its flexibility with cluster shapes. Steps include:
1. Create an adjacency matrix.
2. Determine the Laplacian matrix.
3. Compute eigenvectors to cluster data points, using K-means with randomly initialized centroids.

## Installation
1. Ensure Python and necessary libraries are installed:
    pip install numpy scipy scikit-learn matplotlib pandas
2. Usage:To run the analysis and model training:
    python breast_cancer_prediction.py
3. Results
    Results include the classification accuracy of each model and visualizations of the feature distributions and model performances. Predictive results demonstrate the models' capabilities in identifying potential malignant or benign tumors.