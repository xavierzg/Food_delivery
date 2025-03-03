# Food Delivery
## Introduction
Food delivery is a courier service in which a restaurant, store, or independent food-delivery company delivers food to a customer. 
An order is typically made either through a restaurant or grocer's website or mobile app, or through a food ordering company. 
The delivered items can include entrees, sides, drinks, desserts, or grocery items and are typically delivered in boxes or bags. 
The delivery person will normally drive a car, but in bigger cities where homes and restaurants are closer together, they may use bikes or motorized scooters.


## Objectives
Correctly categorize and clean data by addressing errors and converting columns with incorrect data types. <br>
Add and remove multiple columns to optimize the dataset for model performance, improving the quality of the data used in training. <br>
Conduct an hyperparameter search and visualize the model's performance across different parameter settings to fine-tune the model for optimal results.

## This repository includes the following:
Performed EDA, feature engineering, hyperparameter tuning, and visualizations to optimize model performance. (Food_delivery.ipynb) <br>
Raw data (train.csv) <br>
## Summary :
We worked with a dataset containing 46,000 labels and 20 features, including the target variable. Some features had incorrect data types, and there were approximately 900 missing values across the features, which we addressed using the KNNImputer. We created additional columns from existing ones to extract relevant information. By analyzing feature correlation and using feature importance from a random forest model, we narrowed down the selection to 11 features. <br>
Next, we trained both a random forest and XGBoost model, applying basic hyperparameter tuning to determine the better option. We employed various visualization techniques, such as parallel coordinate plots and heatmaps, to evaluate model performance, checking for overfitting or underfitting and optimizing the hyperparameters accordingly. Ultimately, we chose XGBoost for our final model and proceeded with extensive hyperparameter tuning to improve performance.
 

## Results
The best model was a XGBoost with hyperparameters {'learning_rate': 0.045, 'max_depth': 10, 'min_child_weight': 10, 'reg_lambda': 100}, and $R^2 = 0.821$

