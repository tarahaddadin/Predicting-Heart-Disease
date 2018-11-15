# Predicting-Heart-Disease

General Guidelines:

This is a machine learning model aiming to predict the probability of the binary class 'heart_disease_present', which represents the probability of a patient having a heart disease present (1), or not (0). The dataset used consists of various measurement on patient health and cardiovascular statistics. 

Data is provided courtesy of the Cleveland Heart Disease Database via the UCI Machine Learning repository.

Summary:

To get my final results I used several algorithims from the sklearn package in order to get my results. The next step was scoring the various models and choosing the one with the best score, which turned out to be the 'Random Forest Regressor'. In order to validate this decision and check how this model works, I used K-Folds Cross Validation with K=10, which pointed out that my model had an average accuracy of 80% and a standard deviation of 0.079. 

Feature Selection: 

For the first itieration I have used all features available. 
For the categorical feature 'thal', I have used One-Hot encoding in order to turn it into numeric values. One hot encoding consists of creating 3 new columns for the 3 unique values in the "thal" column with binary values for each.
In addition, I have used the binning method in order to turn the 'age' feature into categorical data. 
Moreover, I evaluated the importances for the features used, which is when I found out the feature 'fixed_defect' had an insignificant importance which is why I decided to drop it and repeat the model. 
