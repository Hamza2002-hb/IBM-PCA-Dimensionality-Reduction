# Principal Component Analysis (PCA) Notes

# What is PCA?

Principal Component Analysis (PCA) is a dimensionality reduction algorithm used to reduce the number of features in a dataset while keeping the most important information.

Instead of using all original features, PCA creates new features called **Principal Components**.

These principal components capture the maximum variance in the data.

---

# Why do we use PCA?

PCA is used to:

- Reduce the number of features
- Remove redundant information
- Reduce noise
- Improve model speed
- Make data easier to visualize
- Improve machine learning performance

---

# Real-Life Example

Imagine you have student data containing:

- Math Marks
- Physics Marks
- Chemistry Marks
- Biology Marks
- English Marks
- Computer Marks
- Attendance
- Assignments

Many of these features may contain similar information.

Instead of using all features, PCA combines the important information into a few principal components.

This reduces complexity while keeping most of the useful information.

---

# PCA Workflow

1. Collect Dataset
2. Standardize the Data
3. Compute Principal Components
4. Calculate Explained Variance
5. Select Top Components
6. Transform Data
7. Train Machine Learning Model

---

# Important Terms

## Feature

A feature is a variable or column in a dataset.

Example:

- Age
- Salary
- Height

---

## Dimension

Dimension means the number of features.

Example:

10 Features = 10 Dimensions

---

## Dimensionality Reduction

Reducing unnecessary features while keeping important information.

---

## Principal Component

A new feature created by PCA.

It is a combination of original features.

---

## Explained Variance

Explained variance tells us how much information each principal component keeps.

Higher explained variance means more useful information.

---

# Advantages of PCA

- Reduces computation time
- Removes correlated features
- Reduces noise
- Makes visualization easier
- Improves model performance
- Works well with high-dimensional datasets

---

# Limitations

- Works only for linear relationships
- Components are harder to interpret
- Some information is lost after reduction

---

# PCA in Scikit-Learn

```python
from sklearn.decomposition import PCA

pca = PCA(n_components=2)

X_pca = pca.fit_transform(X_scaled)
```

---

# Important Parameters

## n_components

Number of principal components to keep.

Example:

```python
PCA(n_components=2)
```

---

# Explained Variance Ratio

```python
pca.explained_variance_ratio_
```

Returns the percentage of information explained by each principal component.

---

# Standardization Before PCA

PCA should usually be applied after scaling the data.

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()

X_scaled = scaler.fit_transform(X)
```

---

# Applications of PCA

- Face Recognition
- Image Compression
- Medical Data Analysis
- Customer Segmentation
- Finance
- Recommendation Systems
- Data Visualization
- Feature Extraction

---

# Comparison

| PCA | t-SNE | UMAP |
|-----|--------|-------|
| Linear | Non-linear | Non-linear |
| Fast | Slow | Fast |
| Feature Reduction | Visualization | Visualization |
| Preserves Variance | Preserves Local Structure | Preserves Local & Global Structure |

---

# Key Takeaways

- PCA stands for Principal Component Analysis.
- PCA is a dimensionality reduction algorithm.
- PCA creates new features called Principal Components.
- PCA keeps the most important information while reducing dimensions.
- PCA works best for linearly correlated data.
- PCA helps reduce noise and computational cost.
- PCA improves visualization and feature extraction.

---

# Skills Learned

- Principal Component Analysis (PCA)
- Feature Reduction
- Explained Variance
- Data Standardization
- Feature Extraction
- Scikit-Learn
- Python
- Machine Learning
- Data Visualization

---

# Author

**Hamza**

Learning Artificial Intelligence and Machine Learning through hands-on projects and practical implementation.

GitHub Repository:
IBM-PCA-Dimensionality-Reduction
