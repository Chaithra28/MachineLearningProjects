# Handwritten Digits Recognition using Data Clustering

This project applies dimensionality reduction and K-Means clustering on image data to visualize clusters and evaluate the optimal number of clusters.

## Requirements

- Python 3.x
- NumPy
- pandas
- matplotlib
- scikit-learn

## Installation

Install the required libraries:  
`pip install numpy pandas matplotlib scikit-learn`

## Usage

### Load Data: 

Load the dataset from `image_test.txt`.

### Dimensionality Reduction:

- Apply TruncatedSVD and PCA.
- Further reduce dimensions using t-SNE.

### K-Means Clustering:

- Perform clustering using a custom K-Means implementation.
- Visualize the clusters.

### Save Predictions: 

Save the clustering results to a CSV file.

### Evaluate Clusters:

Plot inertia to determine the optimal number of clusters.
