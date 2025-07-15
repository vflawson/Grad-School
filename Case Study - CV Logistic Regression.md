# Case-Study---CV-Logistic-Regression-with-Threshold-Optimization-on-Fertility-Dataset
Machine learning in python case study to predict fertility (from the UCI database) and optimize cost function/threshold using cross validation

Fertility data from the UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Fertility

In this case study, the goal is to create a classification model to predict whether a patient is infertile based on their risk factors 
(age, previous diseases, smoking status, drinking status, etc.). 

First, categorical data such as smoking status and previous dissease columns are dummified, following one hot encoding.

The data is then split to include one dataframe for features (x variables) and one for the label (y variable).

The business context and assessment of model errors is assessed in order to establish a cost function to minimize the risk of false negative
errors (patient is diagnosed as fertile when in fact are infertile).

Next, the cost function is formally defined in order to incorporate into a cross-validated logistic regression model.

Using the sklearn statified K fold model, 10 logistic regression models are generated and the cost function of the classification results
is assessed on 100 different threshold levels (0 to 1, with a 0.01 step).

Finally, the 10 different logistic regression models are assessed to determine the optimal threshold level for minimizing the defined
cost function. In this case, 0.43 threshold level and $600 cost function was determined across the 10 folds.
