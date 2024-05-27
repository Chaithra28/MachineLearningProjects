# Overview

This repository contains Python code for analyzing movie data using pandas, numpy, and scikit-learn libraries. Below is an overview of the functionalities and usage of the code.

# Data Loading and Exploration

- Purpose: Load movie data from a CSV file and perform initial data exploration.
- Functionality:
  - Loads data from 'datasets/rotten_tomatoes_movies.csv'.
  - Displays the first few rows of the dataframe using `movies_df.head()`.
  - Checks for missing values using `movies_df.isnull().sum()` and generates descriptive statistics using `movies_df.describe()`.
   
# Data Preprocessing and Visualization

- Purpose: Preprocesses data and visualizes key features.
- Functionality:
  - Handles missing values in certain columns.
  - Converts categorical features into numerical using one-hot encoding.
  - Plots bar charts for 'content_rating' and 'audience_status' using `matplotlib`.
    
# Model Training and Evaluation

- Purpose: Trains and evaluates machine learning models for movie rating prediction.
- Functionality:
  - Prepares features and target variable for classification.
  - Splits the data into training and testing sets using `train_test_split`.
  - Trains a Decision Tree Classifier and Random Forest Classifier.
  - Evaluates models using accuracy score, classification report, and confusion matrix.
  - Visualizes feature importance for the Random Forest model using bar charts.
    
# Usage

- Clone or download the repository.
- Install required libraries (`pandas`, `numpy`, `matplotlib`, `scikit-learn`).
- Run the Python notebook in your preferred environment like jupyter notebook or google colab.
