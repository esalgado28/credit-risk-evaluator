# supervised_ml_challenge
Eddy's folder for supervised machine learning homework 

## Supervised Machine Learning Homework - Predicting Credit Risk
The goal here is to build a machine learning model that can predict wether a loan from LendingClub will become high risk or not. The data includes over 80 features including some of which are categorical. The data used for building the models can be found in the two CSVs:
- `2019loans.csv` (used for training)
- `2020Q1loans.csv` (testing data)

The data was undersampled in order to have equal amounts of high risk and low risk loans. 

### Machine Learning Models
I built and compared two supervised learning models - logistic regression and a random forest classifier. When trained on the unscaled data, the logistic regression model failed to converge and ended up only performing slighly better than a coin toss. The random forest classifier did marginally better at predicting, but was overfitting. 

The data was then scaled using a standard scaler, and the logistic regression model improved significantly to a testing accuracy of about 77%. The random forest classifier, on the other hand, did not improve at all which is interesting. See `Credit_Risk_Evaluator.ipynb`.
