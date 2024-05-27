# Overview
This project implements logistic regression from scratch to predict heart disease from given dataset. It also provides a comparison with the logistic regression implementation from the sklearn library.

# Prerequisites
- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - sklearn
  - time

Install the required libraries using pip:  
`pip install numpy pandas scikit-learn`

# Files

`train.csv`: Training dataset containing features and target labels.  
`test.csv`: Test dataset containing features for prediction.  
`prediction1.csv`: Output file with predictions using custom logistic regression implementation.  
`prediction2.csv`: Output file with predictions using sklearn logistic regression implementation.  

# Code Explanation

## Data Preparation

- Load the training data from train.csv.
- Replace the target labels -1 with 0.
- Split features and target labels:
  - `X_train`: Features matrix.
  - `Y_train`: Target vector.
- Add an intercept column to `X_train`.
- Compute the mean and standard deviation of `X_train`.

## Logistic Regression Implementation

- Sigmoid Function: Compute the sigmoid of z.
- Cost Function: Calculate the logistic regression cost.
- Gradient Calculation: Compute the gradient of the cost function.
- Logistic Regression: Train the logistic regression model using gradient descent.
  - Normalize the feature matrix.
  - Initialize weights.
  - Iteratively update weights until convergence or reaching maximum iterations.
  - Calculate classification error on the training set.
- Training: Train the logistic regression model using the training data.
- Prediction: Predict on the test data using the trained weights.

## Model Training and Evaluation

- Train the logistic regression model from scratch and measure the time taken.
- Compute the training classification error.
- Predict on the test data and save the predictions to `prediction1.csv`.

## Logistic Regression using `sklearn`

- Split the training data into training and validation sets.
- Standardize the features using `StandardScaler`.
- Train the logistic regression model using `sklearn`'s `LogisticRegression`.
- Measure the time taken to train the model.
- Predict on the validation set and compute the accuracy.
- Predict on the test data and save the predictions to `prediction2.csv`.

## Running the Code

Ensure the `train.csv` and `test.csv` files are in the same directory as the script.

Run the script:

`python script_name.py`

## Output

`prediction1.csv`: Predictions using the custom logistic regression implementation.  
`prediction2.csv`: Predictions using sklearn logistic regression implementation.
