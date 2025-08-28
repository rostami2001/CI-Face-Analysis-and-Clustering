# CI-Face-Analysis-and-Clustering

This repository contains the implementation of a computational intelligence project focused on extracting facial features from celebrity images, selecting relevant features, performing clustering, and visualizing the results. This was my first project in the Computational Intelligence course at Ferdowsi University of Mashhad, completed in Fall 2024.

## Project Overview
The goal of this project is to cluster images of celebrities based on extracted facial features such as eye color, skin color, and other binary attributes (e.g., arched eyebrows, big lips). The process includes:
- **Feature Extraction**: Detecting faces using MTCNN, extracting skin and eye colors from images, and appending them to a CSV dataset.
- **Feature Selection**: Computing correlations between features and selecting the top ones using a correlation matrix and threshold.
- **Clustering**: Applying algorithms like KMeans, DBSCAN, and MeanShift, with hyperparameter tuning and evaluation using metrics like silhouette score.
- **Visualization**: Reducing dimensions with PCA and plotting clusters, along with heatmaps for feature analysis and similar image comparisons.

The dataset consists of ~50,000 celebrity images with pre-annotated features, plus a test set of 100 images. Features are binary-encoded (-1 or 1) where applicable.

## Dataset
- The main dataset (celebrity images and features CSV) can be downloaded from this [Google Drive link](https://drive.google.com/drive/folders/124vdZV7BAl6tNdv-33UtRWfNpVSs-YEn).
- `features.csv`: Main features dataset with extracted eye and skin colors.
- `test_features.csv`: Test features dataset.
- `test.zip`: Zip file containing 100 test images.

For detailed analysis, refer to `document.pdf`.
