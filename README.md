# Predicting Income Using Classification and Clustering Models

## Overview
This project applies data preprocessing, classification models (Logistic Regression and Support Vector Machine), and K-Means clustering to predict whether an individual earns more than $50k annually. The dataset used is from the US Census, which includes various demographic features.

## What
The project involves:

1. **Data Preprocessing**: Cleaning and preparing the data for machine learning models by handling missing values, encoding categorical variables, and normalizing the dataset.
2. **Classification Models**: 
   - Logistic Regression: A simple linear model used to predict the income category.
   - Support Vector Machine (SVM): A more powerful classification model to predict income based on demographic features.
3. **K-Means Clustering**: Unsupervised learning approach to group the dataset based on similarities, and evaluating the accuracy of clustering against the actual income labels.

The main goal is to understand how different machine learning models can be used to predict income and how unsupervised methods like clustering can reveal patterns in the data.

## How
1. **Data Loading and Preprocessing**: 
   - The dataset is loaded from a CSV file.
   - Missing values and duplicate entries are handled.
   - Categorical variables like `education`, `sex`, and `workclass` are encoded appropriately, with ordinal values for `education` and dummy coding for other categories.
   - The dataset is split into training and testing sets, and features are normalized.
   
2. **Modeling**:
   - **Logistic Regression** and **SVM** are trained using the training set with 10-fold cross-validation to evaluate performance.
   - The models are fine-tuned by adjusting parameters to improve accuracy.
   - The test set is used to evaluate the final performance of the models.
   
3. **Clustering**:
   - K-Means clustering is applied to the normalized features.
   - The number of clusters is determined by the number of classes in the target variable (`income`).
   - The prototype of each cluster is extracted, and the accuracy of clustering is evaluated by comparing cluster assignments with the true income labels.
   
## Why
The goal of this project is to demonstrate a solid understanding of various machine learning techniques:

1. **Classification Models**:
   - Logistic Regression provides a baseline for a simple predictive model.
   - SVM offers a more complex and flexible model for non-linear classification tasks.

2. **Clustering**:
   - K-Means clustering is used to discover inherent groupings in the dataset, without using the target variable. This can help reveal patterns that might not be obvious with supervised learning alone.

3. **Comparative Analysis**:
   - By comparing the results of the classification models with the results from clustering, the project helps to highlight the strengths and weaknesses of each approach in predicting income levels.
   
By investigating the similarities and differences in clusters and prototypes, this project provides deeper insights into the structure of the data and the potential for both supervised and unsupervised learning in predictive tasks.


