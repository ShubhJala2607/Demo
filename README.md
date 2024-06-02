## ML Model

It is a repositry having ML model Brast cancer based on the Breast Cancer Wisconsin (Diagnostic) dataset.

## 2 Models 
ShubhJala_model_V1- Logistic Regression
ShubhJala_model_V2- Random Forest Classifier

## Dataset

The dataset used is the Breast Cancer Wisconsin (Diagnostic) dataset, Available on UCI Machine Learning Repository.

- Features: 30 numeric features
- Target: Binary classification (Malignant, Benign)

## Setup and Installation
To run the analysis, you need to have Python installed along with the following libraries:
PIP install pandas scikit-learn ucimlrepo

## Fetch Dataset:  
Dataset is fetched from the UCI machine learning Repository using 'ucimlrepo' libraries.

## Data Splitting: 
The data is split into training and testing sets.
Training set: 70% of the data

## Data Standardization: 
The features are standardized to have zero mean and unit variance.

## Model Training: 
A Logistic Regression model and Random Forest Classifier model are trained on the standardized training data.

## Model Evaluation: 
The model's performance is evaluated using accuracy and classification report metrics.

## Result:
Accuracy: The Accuray of the Logistic Regression model and Random Forest Classifier model on the test dataset.


