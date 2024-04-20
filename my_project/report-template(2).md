# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE
Barak Diker
## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
I have needed to test different models like ’GBM’ (LightGBM) ‘CAT’ (CatBoost) ‘XGB’ (XGBoost) ‘RF’ (random forest) ‘XT’ (extremely randomized trees) ‘KNN’ (k-nearest neighbors) ‘LR’ (linear regression) ‘NN_TORCH’ (neural network implemented in Pytorch) ‘FASTAI’ (neural network with FastAI backend) ‘AG_AUTOMM’ 
and from them select the one that fits best 

### What was the top ranked model that performed?
NN_TORCH

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I have seen that the minutes doesnt change so it won't add any more information but 
the hour is changing and it is correlated with the count value . So it's vital information for the prediciton 

### How much better did your model preform after adding additional features and why do you think that is?
There was high correlation between count and the current hour 

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
didn't inprove by much 

### If you were given more time with this dataset, where do you think you would spend more time?
I would change the learning rate , maybe remove some fields

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|’GBM’|‘CAT’|‘RF’|1.8|
|add_features|’GBM’|‘LR’|‘AG_AUTOMM’ |0.53|
|hpo|‘NN_TORCH’|‘LR’|‘AG_AUTOMM’|0.51|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
