# CryptoClustering Challenge

## Overview

In this challenge, you will leverage your Python and unsupervised learning skills to predict the impact of 24-hour or 7-day price changes on cryptocurrencies.

### Before You Begin

- Create a new repository named `CryptoClustering`.
- Clone the repository to your computer.
- Ensure to push your changes to GitHub regularly.

## Instructions

### Step 1: Setup

- Rename the `Crypto_Clustering_starter_code.ipynb` to `Crypto_Clustering.ipynb`.

### Step 2: Load and Visualize the Data

- Load `crypto_market_data.csv` into a pandas DataFrame.
- Obtain summary statistics and visualize the data.

### Step 3: Data Preparation

- Normalize the dataset using `StandardScaler()` from scikit-learn.
- Create a new DataFrame with the scaled data, setting the `coin_id` as the index.

### Step 4: Elbow Method

- Determine the optimal number of clusters (k) using the elbow method.
  1. Generate a range of k values from 1 to 11.
  2. Compute inertia for each k value.
  3. Plot these values to identify the elbow point, indicating the optimal k.

### Step 5: K-means Clustering

- Apply K-means clustering using the optimal k value determined.
- Predict clusters for the cryptocurrencies and append these to the original dataset.
- Visualize the clusters using a scatter plot via hvPlot.

### Step 6: PCA Optimization

- Implement PCA to reduce features to three principal components.
- Examine the explained variance.
- Create a DataFrame with PCA data, indexing by `coin_id`.

### Step 7: PCA-based Clustering

- Repeat the clustering process using PCA-reduced data.
- Visualize the new clusters with hvPlot.

### Step 8: Comparative Analysis

- Assess the impact of feature reduction on clustering by comparing results from the original and PCA-reduced data sets.

## References

- [Scikit-learn KMeans](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
- [Scikit-learn PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
- [Scikit-learn make_blobs](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_blobs.html)
- [hvPlot Scatter](https://hvplot.holoviz.org/reference/pandas/scatter.html)
