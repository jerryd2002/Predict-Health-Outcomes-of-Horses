# Predict_NYC_Taxi_TripTime

* This project focuses on prediciting the trip duration of a taxi cab in NYC (New York City), through the usage of Machine Learning (ML)
* Link: https://www.kaggle.com/competitions/nyc-taxi-trip-duration
  
## Overview

  * **Definition of the tasks / challenge**  Ex: The task at hand is to predict the trip time in seconds, in New York City with machine learning (ML) techniques implementing linear regression to predict the trip time. The challenege uses RMSE (Root-Mean-Squared Errror) between the predicted model and that of the tested model. The challenege is trying to get a low RMSE score, in that our united being measured and predicted the deviation is low.
  * **Your approach** Ex: The appproach we used was using Machine Learning, linear regression model to find a reliable linear regression equation, coefficient and intercept that can help us predict the trip duration.
  * **Summary of the performance achieved** Ex: Our best model was able to predict the next NYC taxi trip duration within 10%, 16% of the time. Much could be done in cleaning the data to ensure the accuracy of predictability increases within a small margin of error. 

## Summary of Workdone

### Data

* Data:
  * Type: float64
    * Input: CSV file consisted of 8 columns which contained pickup and dropoff time along with others.
  * Size: 90mb
  * Instances (Train, Test, Validation Split):
  * Train: Contained 1458644 trip records but reduced to 80,000 trip records
  * Test: 20,000 trips
  * Validation Split: 80% was used as training, and 20% was used as testing

#### Preprocessing / Clean up

* Due to possible outliers in the training data, we removed possible outliers via, IQR and Upper and Lower Bound limits
* Created 2 new columns, "diff_longitude" and "diff_latitude" for the difference of the longitude and latitude between the test and train, and absolute values of the difference.
* Standardizing the feature in order for the data values to be more accurate.

#### Data Visualization

* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/d4878813-3d5b-4f11-bb07-d0e1fc466c5f)
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/cfe9b880-9402-406c-b38d-57ba80b30543)
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/e93b8de3-85be-46ca-9554-ce88d50fc6a3)
*![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/88c27193-98e3-4c36-b1fd-e48322c8a16d)

* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/c22bea9d-c6b3-4ad8-8ddc-d3aa978a099b)
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/82753088-bbf9-4413-bc91-79fb6b691260)



### Problem Formulation

* Define:
  * Input / Output
  * Models
    * Describe the different models you tried and why.
  * Loss, Optimizer, other Hyperparameters.

### Training

* Describe the training:
  * How you trained: software and hardware.
  * How did training take.
  * Training curves (loss vs epoch for test/train).
  * How did you decide to stop training.
  * Any difficulties? How did you resolve them?

### Performance Comparison

* Clearly define the key performance metric(s).
* Show/compare results in one table.
* Show one (or few) visualization(s) of results, for example ROC curves.

### Conclusions

* State any conclusions you can infer from your work. Example: LSTM work better than GRU.

### Future Work

* What would be the next thing that you would try.
* What are some other studies that can be done starting from here.

## How to reproduce results

* In this section, provide instructions at least one of the following:
   * Reproduce your results fully, including training.
   * Apply this package to other data. For example, how to use the model you trained.
   * Use this package to perform their own study.
* Also describe what resources to use for this package, if appropirate. For example, point them to Collab and TPUs.

### Overview of files in repository

* Describe the directory structure, if any.
* List all relavent files and describe their role in the package.
* An example:
  * utils.py: various functions that are used in cleaning and visualizing data.
  * preprocess.ipynb: Takes input data in CSV and writes out data frame after cleanup.
  * visualization.ipynb: Creates various visualizations of the data.
  * models.py: Contains functions that build the various models.
  * training-model-1.ipynb: Trains the first model and saves model during training.
  * training-model-2.ipynb: Trains the second model and saves model during training.
  * training-model-3.ipynb: Trains the third model and saves model during training.
  * performance.ipynb: loads multiple trained models and compares results.
  * inference.ipynb: loads a trained model and applies it to test data to create kaggle submission.

* Note that all of these notebooks should contain enough text for someone to understand what is happening.

### Software Setup
* List all of the required packages.
* If not standard, provide or point to instruction for installing the packages.
* Describe how to install your package.

### Data

* Point to where they can download the data.
* Lead them through preprocessing steps, if necessary.

### Training

* Describe how to train the model

#### Performance Evaluation

* Describe how to run the performance evaluation.


## Citations

* Provide any references.






