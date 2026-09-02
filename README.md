# 🚢 Titanic Survival Prediction

A machine learning classification project that predicts whether a passenger survived the Titanic disaster based on passenger characteristics.

The project explores the complete machine learning workflow, including data preprocessing, feature engineering, model training, hyperparameter tuning, evaluation, and comparison.

## Overview

Using the Titanic dataset, I trained and compared three machine learning classification models:

- Random Forest
- Gradient Boosting
- Logistic Regression

The goal was to determine which model could most effectively predict passenger survival.

## Data Preprocessing

Before training the models, several preprocessing and feature engineering techniques were applied:

- Removed irrelevant features such as Passenger ID, Name, Ticket, and Cabin
- Handled missing values in the dataset
- Used KNN Imputation to estimate missing Age values
- Converted categorical features into numerical representations
- Applied one-hot encoding to the Embarked feature
- Created a new `FamilySize` feature
- Split the dataset into 80% training and 20% validation data

## Models

### Random Forest

A Random Forest classifier was trained and manually tuned using parameters including:

- `n_estimators = 600`
- `max_depth = 7`
- `min_samples_split = 5`

### Gradient Boosting

A Gradient Boosting classifier was trained using:

- `n_estimators = 600`
- `learning_rate = 0.1`
- `max_depth = 7`

### Logistic Regression

A Logistic Regression model was also trained to provide a simpler baseline for comparison.

Key parameters included:

- `C = 0.5`
- `max_iter = 600`

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Correlation Heatmaps

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Random Forest | 82.12% | 83.87% | 70.27% | 76.47% |
| Gradient Boosting | **83.24%** | 81.44% | **77.03%** | **79.17%** |
| Logistic Regression | 81.01% | 78.57% | 74.32% | 76.39% |

**Gradient Boosting achieved the best overall performance**, with the highest accuracy, recall, and F1 score among the three models.

Random Forest achieved the highest precision.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab

## Key Concepts

- Machine Learning
- Binary Classification
- Data Cleaning
- Feature Engineering
- KNN Imputation
- One-Hot Encoding
- Train/Validation Splitting
- Hyperparameter Tuning
- Model Evaluation
- Data Visualization

## Dataset

The project uses the Titanic dataset from the Kaggle **Titanic: Machine Learning from Disaster** competition.

## Project Purpose

This project was developed to gain hands-on experience with the complete machine learning pipeline, from preprocessing raw data to training, tuning, evaluating, and comparing multiple classification models.
