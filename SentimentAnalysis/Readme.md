# Sentiment Analysis on Customer Reviews
This project focuses on building a sentiment analysis model to classify customer reviews as positive or negative. The model is trained using Logistic Regression and optimized with GridSearchCV. The text preprocessing includes tokenization, removal of punctuation and stopwords, and lemmatization.

# Prerequisites
Python 3.x
Required libraries:
pandas
nltk
textblob
scikit-learn

# Data Preparation

## Load Training Data: 

- The training data is loaded from a file named `train_file.dat`. 
- Each line in this file contains a label (1 for positive and -1 for negative) and a review.

# Text Preprocessing: 

The reviews are preprocessed using the following steps:

- Tokenization: Splitting the text into words.
- Contraction handling: Expanding common contractions (e.g., "don't" to "do not").
- Lowercasing: Converting all words to lowercase.
- Punctuation removal: Removing punctuation marks.
- Number removal: Removing numerical values.
- Stopword removal: Removing common words that do not carry significant meaning (e.g., "the", "is").
- Lemmatization: Converting words to their base forms (e.g., "running" to "run").
  
# Model Training

- Split Data:
  The data is split into training and validation sets using an 90-10 split.

- Pipeline and GridSearchCV:

  - A pipeline is created with `TfidfVectorizer` for feature extraction and `LogisticRegression` for classification.
  - `GridSearchCV` is used to find the best hyperparameters for the model. The parameters tuned include the maximum number of features, n- 
    gram range, regularization strength (C), penalty type (l1 or l2), and the maximum number of iterations.
  
- Training and Validation: 

  - The model is trained using the training set, and its performance is validated on the validation set. The best hyperparameters and the 
    best model estimator are obtained from `GridSearchCV`.

# Evaluation

- Best Hyperparameters: The best hyperparameters found by `GridSearchCV` are printed.
- Model Performance: The accuracy of the best model is evaluated on the validation set.
  
# Predictions on Test Data

- Load Test Data: Test data is loaded from a file named `1675198994_6787539_1567602457_126649_test.dat`.

- Text Preprocessing: The same preprocessing steps used for the training data are applied to the test data.

- Predictions: The trained model is used to predict the sentiment of the test reviews.

- Save Predictions: The predictions are saved to a file named `predictions.dat`.

# Usage

- Ensure all required libraries are installed.
- Place the training data file (`train_file.dat`) and test data file (`1675198994_6787539_1567602457_126649_test.dat`) in the working 
  directory.
- Run the script to preprocess data, train the model, evaluate its performance, and make predictions on the test data.
