# Medicalcost Regression
Build regression model with random forest and try to hyperparameter tuning with random search, then predict medical insurance cost.
Dataset from kaggle: [Medical cost dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)

## Data Pre-processing
* Check null values
* Check distribution of dataset and find outliers
* Convert category features into numberical features with LabelEncoder
* Test-Test split with 70:30

## Hyperparameter tuning
Tuning hyperparameter with random search.
Here's my set of my best parms: n_estimators= 144, min_samples_split= 2, min_samples_leaf= 7, max_features= 'auto', max_depth= 4, bootstrap= True

## Model results
Here's my result with testing data.
 | Model     | MSE           | RMSE      | R2     |
 | --------  | ------------- | --------- | -----  |
 | base_rf   | 23318975.4703 | 4828.9725 | 0.8221 |
 | tuning_rf | 18962642.5743 | 4354.6116 | 0.8553 |
