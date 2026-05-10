# Project 5 Summary — Dimensionality Reduction (PCA, t-SNE, Clustering)

## Project Overview

In this project, I learned how dimensionality reduction works and why it is important in machine learning.

The main goal was to reduce high-dimensional data into a smaller number of dimensions while keeping as much useful information as possible.

I worked with:

* PCA (Principal Component Analysis)
* t-SNE
* KMeans Clustering
* Silhouette Score
* Data visualization

The dataset used was the Wine dataset from scikit-learn.

---

# What I Learned

## 1. Dimensionality Reduction

Dimensionality reduction is the process of reducing the number of features in a dataset.

This is useful because:

* High-dimensional data is difficult to visualize
* Too many features may introduce noise
* Models can become slower and more complex
* Some features may contain overlapping information

I learned that dimensionality reduction can help:

* simplify the dataset
* improve visualization
* reduce overfitting
* improve computational efficiency

---

# 2. PCA (Principal Component Analysis)

PCA creates new features called principal components.

These components are combinations of the original features and are designed to capture the maximum amount of variance in the data.

Important concepts learned:

* PCA is a linear dimensionality reduction method
* PCA depends heavily on variance
* Features must be scaled before applying PCA
* Principal components are ordered by importance

I reduced the dataset from 13 dimensions down to 2 dimensions.

---

# 3. Explained Variance Ratio

I learned how to measure how much information is preserved after dimensionality reduction.

The explained variance ratio shows how much variance each principal component captures.

Example:

* PC1 may capture 36% of the variance
* PC2 may capture 19%

This means the first two components together preserve about 55% of the original information.

I also learned how to use cumulative explained variance graphs to determine how many components should be kept.

---

# 4. Data Visualization

I visualized the PCA-transformed data using scatter plots.

This helped reveal:

* cluster separation
* relationships between classes
* overall data structure

I learned that dimensionality reduction is extremely useful for visual exploration.

---

# 5. t-SNE

I learned that t-SNE is another dimensionality reduction technique.

Unlike PCA:

* t-SNE is non-linear
* t-SNE is mainly used for visualization
* t-SNE preserves local structure better
* t-SNE usually creates clearer cluster separation

I compared PCA and t-SNE visualizations.

Main differences:

| PCA                        | t-SNE                         |
| -------------------------- | ----------------------------- |
| Linear                     | Non-linear                    |
| Faster                     | Slower                        |
| Good for feature reduction | Best for visualization        |
| Preserves variance         | Preserves local relationships |

---

# 6. KMeans Clustering

I applied KMeans clustering to the PCA-transformed dataset.

I learned:

* how clustering works without labels
* how KMeans groups similar data points together
* how PCA and clustering are commonly used together

The clustering result was visualized using scatter plots.

---

# 7. Silhouette Score

I learned how to evaluate clustering quality using Silhouette Score.

Interpretation:

* score near 1 → strong clustering
* score near 0 → overlapping clusters
* negative score → poor clustering

This helped me understand how to evaluate unsupervised learning models.

---

# Important Interview Concepts Learned

## Why scaling is important before PCA

PCA depends on variance.

Without scaling, features with larger values can dominate the principal components.

---

## Difference between PCA and t-SNE

PCA:

* used for dimensionality reduction
* faster
* interpretable
* linear

t-SNE:

* mainly used for visualization
* captures complex non-linear patterns
* slower
* less interpretable

---

## What is a principal component?

A principal component is a new feature created from a combination of the original features that captures the maximum variance.

---

## Does PCA always improve model performance?

No.

PCA can:

* reduce noise
* reduce overfitting
* improve speed

But it can also remove useful information.

---

# Skills Practiced in This Project

* Data preprocessing
* Feature scaling
* Dimensionality reduction
* Visualization
* Clustering
* Model evaluation
* Unsupervised learning concepts
* Interview explanations

---

# Technologies and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* scikit-learn

---

# Possible Improvements and Next Steps

## 1. Build a Streamlit Application

Possible features:

* Upload custom datasets
* Select number of PCA components
* Visualize PCA results interactively
* Run clustering automatically
* Show explained variance graphs
* Compare PCA vs t-SNE visually

This would make a strong portfolio project.

---

## 2. Add More Clustering Algorithms

Future improvements:

* DBSCAN
* Hierarchical Clustering
* Gaussian Mixture Models

This would allow comparison between clustering methods.

---

## 3. Add UMAP

UMAP is another dimensionality reduction method.

It is often faster than t-SNE while preserving local structure well.

---

## 4. Hyperparameter Tuning

Possible tuning:

* number of PCA components
* number of clusters in KMeans
* perplexity in t-SNE

---

## 5. Apply to Real-World Datasets

Possible datasets:

* customer segmentation
* fraud detection
* image embeddings
* recommendation systems
* genomic datasets

---

# Final Reflection

This project helped me understand how to simplify and visualize complex datasets using dimensionality reduction techniques.

I learned both the mathematical intuition and practical implementation of PCA and t-SNE, as well as how clustering can be combined with dimensionality reduction for better analysis and visualization.

This project also strengthened my understanding of:

* preprocessing
* visualization
* unsupervised learning
* feature engineering
* interview-level machine learning concepts
