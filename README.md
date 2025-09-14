# Credit-Score-Classification
This project predicts whether a credit card client will default on payment using machine learning. It applies multiple ML algorithms, evaluates performance, and compares their results.


# Dataset

Source: UCI Machine Learning Repository — Default of Credit Card Clients Dataset
File: default of credit card clients.xls
Records: 30,000 clients
Target: default (0 = No Default, 1 = Default)


# Project Workflow

1. Data Preprocessing
Handle missing values
Encode categorical variables
Scale numerical features (StandardScaler)

2. Exploratory Data Analysis (EDA)
Distribution plots of features
Correlation heatmap
Class balance check

3. Model Training
We trained and evaluated the following algorithms:
Logistic Regression
kNN (K-Nearest Neighbors)
SVM (Support Vector Machine)
Random Forest
XGBoost

4. Evaluation Metrics
Accuracy
Precision, Recall, F1-Score
Confusion Matrix
ROC-AUC Curve


# Results

| Model               | Accuracy | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) | ROC-AUC |


| ------------------- | -------- | ------------------- | ---------------- | ------------------ | ------- |


| Logistic Regression | 0.81     | 0.69                | 0.24             | 0.36               | \~0.76  |


| kNN                 | 0.79     | 0.55                | 0.35             | 0.43               | \~0.69  |


| SVM                 | 0.82     | 0.67                | 0.34             | 0.45               | \~0.75  |


| Random Forest       | 0.81     | 0.64                | 0.37             | 0.47               | \~0.74  |


| XGBoost             | 0.81     | 0.62                | 0.36             | 0.46               | \~0.73  |


* Best Overall Model: Logistic Regression (simple & robust baseline)
* Best Balanced Model: Random Forest / SVM


# Future Improvements

Try LightGBM / CatBoost (alternative boosting algorithms)


Hyperparameter tuning with GridSearchCV


Add feature importance analysis


Deploy with Streamlit or Flask

# References

UCI Credit Card Dataset - https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients


Scikit-learn, XGBoost documentation
