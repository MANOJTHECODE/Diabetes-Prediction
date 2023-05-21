# Diabetes-Prediction

## Introduction
This project aims to develop a predictive model for diabetes detection using the diabetes dataset. The dataset contains various features such as pregnancies, glucose level, blood pressure, skin thickness, insulin, BMI, diabetes pedigree function, and age. The project involves data collection and analysis, data standardization using StandardScaler, train-test split, training a support vector machine (SVM) classifier, evaluating the model's accuracy, and creating a predictive system to classify a person as diabetic or non-diabetic based on input data. The model achieves an accuracy score of around 78% on the training data and 77% on the test data.

## explanation of code
The given code performs the task of predicting diabetes using a support vector machine (SVM) classifier. Let's break down the code into different sections:

Data Collection and Analysis:-

The code imports necessary libraries such as numpy, pandas, and scikit-learn modules.
It loads a diabetes dataset from a CSV file and displays the first few rows, last few rows, shape, and statistical summary of the dataset.
The code also shows the count of non-diabetic and diabetic instances in the dataset, along with the mean values of features grouped by the outcome.
Data Preprocessing:

The code separates the features (X) and labels (Y) from the dataset.
It then applies data standardization using the StandardScaler from scikit-learn, which scales the features to have zero mean and unit variance.
The standardized features are stored in the X variable, and the original labels are stored in the Y variable.
Train-Test Split:

The code splits the standardized data into training and testing sets using the train_test_split function from scikit-learn. It uses 80% of the data for training and 20% for testing, while ensuring that the proportion of diabetic and non-diabetic instances is preserved in both sets.
Model Training and Evaluation:

The code creates an SVM classifier with a linear kernel using the svm.SVC class from scikit-learn.
It then trains the classifier on the training data using the fit method.
The code evaluates the model's accuracy on both the training and test data by comparing the predicted labels with the actual labels.
The accuracy scores are printed, indicating the proportion of correct predictions made by the model.
Predictive System:

The code demonstrates how to use the trained SVM classifier to make predictions on new, unseen data.
It defines an input data point and standardizes it using the previously fitted StandardScaler.
The standardized data is passed to the classifier's predict method to obtain the predicted label.
Finally, based on the predicted label, the code outputs whether the person is diabetic or not.
Overall, this code provides a basic implementation of training an SVM classifier on a diabetes dataset and using it for prediction. It serves as a starting point for further exploration and improvement in terms of model selection, hyperparameter tuning, and additional data preprocessing or feature engineering techniques.
