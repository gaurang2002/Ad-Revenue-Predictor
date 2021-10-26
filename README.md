# Ad Revenue Prediction 

## EDA/Feature Engineering
1. Given dataset is small so we concatenate the train and test dataset and performed EDA on it.
2. We have added three new columns:
  - CPC = Cost per clicks
  - CTR = No of clicks performed / (per impression)
  - COA = Cost / Conversion
3. We have used label encoding on  the categorical feature columns.
4. We tried to scale dataset by using min-max scaler but we did't got desired result so we decided to drop this idea.
5. As the dataset is of time series we cannot randomly split the dataset into training dataset and validation dataset so we decided to split the data contigously.

## Models and Notebooks
1. We have used three models  XgBoost, Linear regression and Random Forest Regressor
2. Initally we were using xgboost with default parameters ,than we tried to hyper tune by two differnet techniques:
  - Optuna for Bayesian Hyperparameter tuning
  - GridSearchCV
  - Out of the above two optuna "Bayesian Hyperparameter tuning" manage to hypertune the parameters more effciently ,we decided to use each prediction as final submission
  - [Revenue Prediction](https://www.kaggle.com/gaurangthakur/revenue-generation)

## Scope for Improvement:
1. Better Feature engineering can be done.
2. Better split size of validation and training dataset could have give better results
3. More efficient eda and how to tackle with the correlation/interdepedence of the columns on eachother
 
