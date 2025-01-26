# Credit Card Fraud Detection - Sampling and Classification


## Project Overview

In this project, different sampling techniques are applied to balance the dataset and evaluate their effect on classification accuracy. The project uses five sampling techniques, followed by five different classifiers to assess the performance of each method.

## Sampling Methods

The following sampling techniques are applied to balance the dataset:

1. **Random Under-Sampling (RUS)**: Reduces the number of majority class samples.
2. **Random Over-Sampling (ROS)**: Increases the number of minority class samples.
3. **SMOTE (Synthetic Minority Oversampling Technique)**: Generates synthetic samples for the minority class.
4. **SMOTE + Tomek Links**: Combines SMOTE with Tomek Links to clean the data by removing overlapping instances.
5. **NearMiss**: An under-sampling technique that selects samples based on the nearest minority class neighbors.

## Classifiers Used

Five classifiers are evaluated to check the effect of resampling methods on model performance:

1. **Logistic Regression**
2. **Random Forest Classifier**
3. **Decision Tree Classifier**
4. **Naive Bayes**
5. **Support Vector Machine (SVM)**

## Evaluation Metrics

The classification accuracy is computed for each sampling method and classifier combination. The results are stored in a CSV file and can be analyzed to identify which resampling method works best with which classifier.

## Files

- **`Creditcard_data.csv`**: Original dataset containing credit card transaction data, with labels indicating fraudulent transactions.
- **`sampling_model_results.csv`**: Results file storing the accuracy of each classifier for each resampling method.
- **Balanced datasets**: After applying each sampling method, the balanced datasets are saved in CSV files (`balanced_method.csv`), such as `balanced_random_under_sampling.csv`, `balanced_smote.csv`, etc.
