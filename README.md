# Penguin Clustering Analysis

This repository contains a project aimed at identifying groups of penguins in Antarctica using clustering techniques. The dataset used for this analysis is `penguins.csv`, which includes various measurements of penguins but lacks species information. The goal is to apply clustering to discover potential groups or species based on the available features.

## Dataset

The dataset `penguins.csv` includes the following columns:
- `culmen_length_mm`: Culmen length in millimeters
- `culmen_depth_mm`: Culmen depth in millimeters
- `flipper_length_mm`: Flipper length in millimeters
- `body_mass_g`: Body mass in grams
- `sex`: Penguin sex (male or female)

## Objective

The task is to cluster the penguins into groups using K-Means clustering, given the lack of species information. Three species are known to inhabit the region: Adelie, Chinstrap, and Gentoo.

## Code Overview

### 1. Data Preprocessing
- Load the dataset and remove rows with missing values.
- Select relevant features for clustering.

### 2. Feature Standardization
- Standardize the features to ensure that all variables contribute equally to the clustering process.

### 3. Clustering
- Apply K-Means clustering with 3 clusters, based on the known species.
- Assign cluster labels to each data point.

### 4. Visualization
- Visualize the clusters using a scatter plot to understand the distribution of clusters based on `culmen_length_mm` and `culmen_depth_mm`.

### 5. Additional Analysis
- Elbow Method: Used to determine the optimal number of clusters by plotting the distortion score for different cluster numbers.
- Silhouette Score: Provides a measure of how well-defined the clusters are.
- Pairplot: Visualizes relationships between features and clusters to gain deeper insights.

## Usage

1. Install Dependencies:
   Make sure you have the required libraries installed. You can use `pip` to install them:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```

2. Run the Analysis:
   Execute the provided Python script to perform clustering and visualization.

3. View Results:
   Check the generated plots for cluster visualization and the elbow method analysis for cluster validation.

## Repository Structure

- `penguins.csv`: The dataset file.
- `penguin_clustering.ipynb`: The main Python script performing clustering and visualization.
- `README.md`: This file, providing an overview and instructions.

## Contributing

Feel free to fork this repository and make your own improvements. Pull requests are welcome!
