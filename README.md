# Heart Disease Classification | Blacksheep Labs

## Project Overview

This project demonstrates an end-to-end supervised machine learning classification workflow using Python and scikit-learn.

The objective is to predict the presence or absence of heart disease using the UCI Cleveland Heart Disease dataset.

The project covers data preparation, model training, hyperparameter tuning, model evaluation, cross-validation, and feature importance analysis.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- scikit-learn
- Google Colab
- GitHub

## Dataset

**Source:** UCI Machine Learning Repository — Cleveland Heart Disease Dataset

- Total samples: 303
- Training samples: 242
- Testing samples: 61
- Input features: 13
- Target: Binary classification (heart disease present or absent)

## Machine Learning Models

Three classification algorithms were explored:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Random Forest Classifier

Hyperparameter tuning was performed using GridSearchCV and RandomizedSearchCV.

The final evaluated model was a tuned Random Forest Classifier.

## Model Performance

### Held-Out Test Results

| Metric | Score |
|---|---|
| Accuracy | 91.80% |
| Precision | 89.66% |
| Recall | 92.86% |
| F1 Score | 91.23% |
| ROC AUC | 0.9675 |

### Cross-Validation Results

Five-fold cross-validation was performed on the training data.

| Metric | Average Score |
|---|---|
| Accuracy | 82.24% |
| Precision | 86.20% |
| Recall | 73.79% |
| F1 Score | 79.05% |
| ROC AUC | 0.8928 |

The difference between cross-validation and held-out test performance illustrates why model evaluation across multiple data splits is important.

## Feature Importance

Random Forest feature importance analysis identified the following top five features:

| Feature | Importance |
|---|---|
| thal | 19.56% |
| cp | 16.76% |
| ca | 16.34% |
| thalach | 11.64% |
| oldpeak | 9.01% |

Permutation importance was also calculated to investigate model reliance on individual features.

Both methods ranked `thal` as the most important feature.

Feature importance represents predictive contribution, not medical causation.

## Machine Learning Workflow

1. Load and inspect the dataset.
2. Clean and prepare features.
3. Split data into training and testing sets.
4. Train and compare classification models.
5. Tune hyperparameters using cross-validation.
6. Evaluate accuracy, precision, recall, F1 score, and ROC AUC.
7. Analyze confusion matrices and ROC curves.
8. Investigate feature importance.
9. Document results and limitations.

## Limitations

- The dataset contains only 303 samples.
- Results may vary across different training and testing splits.
- The held-out test set was examined during the educational workflow.
- External validation has not been performed.
- The model is an educational demonstration and is not suitable for clinical diagnosis or medical decision-making.

## Author

**Blacksheep Labs**

Machine Learning | Python | Data Science | Artificial Intelligence
