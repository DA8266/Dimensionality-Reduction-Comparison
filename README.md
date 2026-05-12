# Dimensionality-Reduction-Comparison

## Project Overview
This project explores the intersection of linear algebra and machine learning by implementing a facial recognition pipeline using the **Labeled Faces in the Wild (LFW)** dataset. The goal was to manually implement dimensionality reduction and compare how different classifiers handle high-dimensional data once it has been projected into a lower-dimensional space.

## Technical Workflow
The project follows a rigorous mathematical approach to feature extraction:
1. **Preprocessing**: Extracted individuals with at least 70 images and flattened image matrices into high-dimensional vectors.
2. **Feature Centering**: Computed the "Average Face" and subtracted it from the dataset to isolate unique facial features.
3. **Dimensionality Reduction (PCA)**: Leveraged centered vectors to construct a covariance matrix and extract eigenvectors, reducing the feature space while retaining critical variance.
4. **Model Training**: Benchmarked a **Support Vector Machine (SVM)** with optimized parameters against a **Logistic Regression** model.

## Key Results & Comparison
<img width="873" height="664" alt="image" src="https://github.com/user-attachments/assets/3337a690-d71d-4d98-b4c2-ec68714a13fe" />

The **SVM** demonstrated superior performance over **Logistic Regression**. Because facial data is inherently non-linear, the SVM’s ability to create non-linear boundaries allowed it to classify images more accurately than the linear constraints of Logistic Regression.

## Libraries Used
* Python
* NumPy
* Pandas
* Scikit-Learn
* Matplotlib
