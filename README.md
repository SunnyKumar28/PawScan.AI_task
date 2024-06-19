Classification with an Academic Success Dataset
This repository contains the code for predicting students' academic success using a dataset that includes various features related to students' background and academic performance. The main objective is to classify the students into three categories: Graduate, Dropout, and Enrolled.

# Obtained Accuracy
The model achieved an accuracy of** 83.47% **on the test dataset.

# Approach
Data Collection and Pre-Processing

Loading the Data: The training and testing datasets were loaded using pandas.
Exploratory Data Analysis: Initial exploration of the datasets to understand the structure and identify any missing values. No missing values were found in the training data.
Data Encoding: The target variable "Target" was encoded to numeric values:
Graduate: 0
Dropout: 1
Enrolled: 2
Data Splitting

The training data was split into training and validation sets using train_test_split with a test size of 20% and stratified sampling to maintain the proportion of each class.
Data Standardization

StandardScaler from sklearn.preprocessing was used to standardize the features by removing the mean and scaling to unit variance.
Model Training and Evaluation

An XGBoost Classifier (XGBClassifier) was used for training the model.
The model was trained on the standardized training data.
The accuracy on the validation set was calculated using accuracy_score, resulting in an accuracy of 83.47%.
Predicting the Target for Test Data

The test data was standardized using the previously fitted StandardScaler.
Predictions were made on the standardized test data.
The numeric predictions were mapped back to their original class names (Graduate, Dropout, Enrolled).
Submission

The predictions were saved to a CSV file in the required format for submission.
# Dependencies
1.pandas
2.numpy
3.scikit-learn
4.xgboost







