# education-type-prediction

## Purpose
The goal of the project was to create a model that predicts a person's education level based on: gender, car ownership, real estate ownership, number of children, income, number of members in the family, source of income, and family status.

## Dataset
Data comes from "Credit Card Approval Prediction" dataset on kaggle.com\
https://www.kaggle.com/datasets/rikdifos/credit-card-approval-prediction?select=application_record.csv

Whole dataset contains 438737 examples\ 
159 outlier observations were dropped\
Train dataset contains 350718 examples\
Test dataset contains 87860 examples\

## Models

1. Logistic regression with L2 regularization
2. SGD Classifier (mini-batch gradient descent optimizer, size of batch = 100, without regularization)
3. Neural network (Adam optimizer, cross-entropy as loss function, PyTorch library)

## Evaluation

| Model               | Accuracy | Recall | F1-score |
| ------------------- | -------- | ------ | -------- |
| Logistic regression | **0.7030**   | 0.6406 | **0.6269**   |
| SGD                 | 0.6919   | **0.7409** | 0.5659   |
| Neural Network      | 0.6998   | 0.6370 | 0.6250   |
