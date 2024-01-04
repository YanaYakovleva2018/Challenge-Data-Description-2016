# Predictive Maintenance Challenge
This repository contains code for a predictive maintenance challenge involving the analysis of multivariate time series data. The task revolves around predicting the remaining operational cycles for engines within a fleet, considering factors such as operational settings, initial wear, and manufacturing variation.

## Code Overview
### Libraries Used

The code utilizes the following Python libraries:

1. pandas for data manipulation
2. numpy for numerical operations
3. random for random sampling
4. scikit-learn for machine learning tasks
5. matplotlib for data visualization
6. statsmodels for statistical modeling
### Execution
The code follows these main steps:

1. Data Loading and Preprocessing:

Loads training data from 'train.txt' and preprocesses it.
Performs rolling mean calculation and splits the data into training and test sets.

2. Backward Feature Elimination:

Uses backward feature elimination to select relevant features for the model.

3. Model Training and Evaluation:

Trains a Random Forest regression model on the training set.
Evaluates the model on the training set and visualizes predictions.
Loads test data from 'test.txt' and preprocesses it.
Evaluates the trained model on the test set.

4. Final Test Set Evaluation:

Loads final test data from 'final_test.txt' and preprocesses it.
Evaluates the trained model on the final test set and visualizes predictions.

5. Results Export:

Saves the predicted RUL results to a CSV file ('predicted_rul_results.csv').
