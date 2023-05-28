# Iris Species Prediction using PCA and K-means Clustering

This project focuses on predicting the species of Iris flowers based on their measurements using the Iris dataset. The Iris dataset is a well-known benchmark dataset in machine learning, consisting of measurements of sepal length, sepal width, petal length, and petal width for three different Iris species: setosa, versicolor, and virginica.

## Project Overview

The main objective of this project is to develop an algorithm that can accurately predict the species of Iris flowers based on their measurements. To achieve this, the project leverages two powerful techniques: Principal Component Analysis (PCA) and K-means clustering.

### Principal Component Analysis (PCA)

PCA is a dimensionality reduction technique that transforms the original features into a lower-dimensional space, capturing the maximum amount of variance in the data. By applying PCA, we can eliminate redundant information and noise, thereby improving the performance of subsequent analysis algorithms.

In this project, PCA is employed to reduce the dimensionality of the Iris dataset. By transforming the original feature space into a reduced-dimensional representation, we can visualize and understand the underlying patterns in the data more effectively.

### K-means Clustering

K-means clustering is an unsupervised machine learning algorithm used for grouping similar data points into distinct clusters. It aims to partition the data into a predetermined number of clusters based on their similarities.

In the context of this project, K-means clustering is applied to the transformed Iris dataset obtained from PCA. By clustering the data points in the reduced feature space, we can identify groups of similar Iris samples.

The K-means algorithm iteratively assigns each data point to the nearest cluster centroid and updates the centroids' positions until convergence is achieved. Once the algorithm converges, each data point is assigned to a specific cluster based on its proximity to the centroid.

To determine the predicted Iris species for each cluster, we consider the majority class label of the data points within that cluster. This allows us to assign a predicted species label to each individual Iris sample based on its proximity to the centroid of the corresponding cluster.

## Project Implementation

The project implementation consists of the following steps:

1. Loading and preprocessing the Iris dataset: The original Iris dataset is loaded and preprocessed, ensuring that the data is in a suitable format for analysis.

2. Applying Principal Component Analysis (PCA): PCA is applied to the dataset, reducing the dimensionality and obtaining a transformed representation of the Iris samples.

3. Performing K-means Clustering: K-means clustering is performed on the transformed dataset, grouping the Iris samples into clusters based on their similarities in the reduced feature space.

4. Assigning Predicted Species Labels: Each individual Iris sample is assigned a predicted species label based on its proximity to the centroid of the corresponding cluster. The majority class label within each cluster is considered for prediction.

5. Evaluating Model Performance: The performance of the Iris species prediction model is evaluated using appropriate metrics, such as accuracy, precision, recall, and F1 score.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository to your local machine.
2. Install the necessary dependencies and libraries as specified in the requirements file.
3. Run the Jupyter notebooks
