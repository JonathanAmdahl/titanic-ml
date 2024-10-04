# Kaggle Titanic Dataset

Created a Neural Network to predict who will (and won't) survive the titanic based on the provided data.

# Scores
On Kaggle, this scored a .79186 which at the time of writing this is #1086 out of 14258 submissions. Making this a top 8% submission

# Time
This was done in one night and the next morning. 

# Data Cleaning and Imputation
Dropped 'cabin' as too many values were missing (however, later extracted deck from it)


Imputed 'age' with XGBoost which improved the accuracy of the model a fair bit


Imputed 'embarked' with mode (only a couple values were missing)

# Training
Implemented K Fold Cross Validation (10 folds) as the testing data does not have a target column. Additionally, was running into some slight overfitting problems which this helped a lot with.
Implemented optuna for hyperparameter tuning

# Learnings
This is one of the first models that I have actually implemented without an accompanying walk-along. This made me a lot more comfortable with the process of implementing a model.

In specific:
-Not getting hung up on making everything perfect initially and just getting working predictions, made me more likely to persevere 


-I realized I worked on hyperparameter tuning WAY too early. However, setting up the foundation for re-using it was still very helpful.


-Realizing the importance of imputation, I spent a lot of time trying to feature engineer when in reality I got much better results focusing on imputation.

# What I would change if I spent more time
-I would try to increase the accuracy of the age imputation


-I would start to spend more effort on hyperparameter tuning