# Kaggle: Predicting Customer Churn Using KNN

This repository contains a notebook-based machine learning project focused on **customer churn prediction** for a Kaggle-style competition.

## What it does

The project trains a churn classifier to predict whether a customer will leave. The implementation centers on a **custom K-Nearest Neighbors (KNN)** model, with additional experimentation around boosting and preprocessing.

## Main ideas in the notebook

- Custom implementation of a **KNN classifier**
- Experimental **AdaBoost-style ensemble** using KNN as the base learner
- Manual preprocessing utilities, including:
  - Min-max scaling
  - handling class imbalance / sampling logic
- Cross-validation for model evaluation
- Generation of a submission file for competition use

## Repository contents

- `assignment5_starter.ipynb` - Main notebook with modeling code and experiments
- `train.csv` - Training data
- `test.csv` - Test data
- `submissions.csv` - Output predictions/submission file

## Approach summary

The notebook suggests a workflow like this:

1. Load training and test data
2. Preprocess features manually
3. Train a custom KNN model
4. Evaluate with cross-validation
5. Tune hyperparameters such as `k`
6. Export predictions for Kaggle submission

There is also evidence of experimentation with weighted learning / ensemble-style extensions through an `AdaBoostKNN` class.

## Run locally

1. Open the notebook in Jupyter or VS Code
2. Make sure the CSV files are in the same directory
3. Run the notebook cells in order

## Why this repo is useful

This project is useful if you want to see:

- a from-scratch KNN implementation for a real prediction task
- how to build a competition workflow inside a notebook
- how to experiment with preprocessing and imbalance handling in tabular ML problems
