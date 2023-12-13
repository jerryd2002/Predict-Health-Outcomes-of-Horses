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
* Pickup Longitude
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/d4878813-3d5b-4f11-bb07-d0e1fc466c5f)
* Pickup Latitude
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/cfe9b880-9402-406c-b38d-57ba80b30543)
*  Dropoff Longitude
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/e93b8de3-85be-46ca-9554-ce88d50fc6a3)
*  Dropoff Latitude
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/88c27193-98e3-4c36-b1fd-e48322c8a16d)
*  Trip Duration
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/7a684a51-8cc2-4ce1-8a08-11311ab66938)
*  Distance Difference of Latitude and Longitude
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/c22bea9d-c6b3-4ad8-8ddc-d3aa978a099b)
*  Actual vs. Adjusted Predicted Trip Durations
* ![image](https://github.com/jerryd2002/Predict_NYC_Taxi_TripTime/assets/98507605/82753088-bbf9-4413-bc91-79fb6b691260)



### Problem Formulation

* Define: The model should be similar to that of hte data that is contained in the sample_submission.zip, through that we train the model.
   * Input/Output:
   * Input: test.zip, train.zip
   * Output: predicted_trip_duration.csv, containing the predicted
*Models:
  *Usage of Linear Regression: Predicted possible trip duration based upon tested and train dataset.

### Training

* Describe the training:
  * Used LinearRegreesion, model was trained under the test and train dataset, in order to predict taxi duration in NYC through utilizing and attempting to replcate the sample_submission.zip, then utilizing RMSE (Root Mean Squared Error) that shows the variance between the model and the data being compared to.
  

### Conclusions

* Given our computed values of RMSE = 844.32 and percentage of perdictability of predictions within 10% error: 15.63%, our model appears to unreliant when compaing to that of the data as we appear to have high variance between them. Most likely, error in the code for the model that caused the high variance, with that most likely comparing incorrectly.

### Future Work

* I would try to improve on my models to reduce the variance, the RMSE score that will help make my models more reliable that allows for its predictions to be used with confidence with other datasets.
* Implying this further into other studies using advanced regression models and error analysis to determine why models are making errors.

## How to reproduce results
 * Clone the repository
 * Download rhe files from the Kaggle Challenege link
 * Unzip the downloaded files, then look at the dataframe of the test.zip and train.zip
 * Remove Outliers in the trip duration of our data set.
 * Visualize the columns necessary to help make trip duration prediction
 * Forms graphs, histogram in this case that visualizes the longitutde, latittude, and trip duration
 * Using the Linear Regression Model from Sklearn to predict.
 * Analyze the predict variance from actual using RMSE and Perctange of Perdictability to insure reliability 
   


### Overview of files in repository

* Jerry_Prediction.ipynb: contains the visulizations, linear regression model, RMSE
* predicted_trip_duration.csv: contains the id and predicted taxi duration to that of id
* result_with_difference.csv: contains the difference of longitude and latitude, dropoff and pickup with time duration 

### Software Setup
* Python 3.7
* Required Packages:
  * Install in terminal
    * Pandas: 'pip install pandas'
    * Numpy: ' pip install numpy'
    * Matplotlib.pyplot: 'pip install matplotlib'
    * Sklearn: 'pip install scikit-learn'
    * import train_test_split, mean_squared_error, LinearRegression, and Standard Scaler in Notebook
      
    * ZipFile: import ZipFile
  

### Data
 * All the data can be downloaded through the Kaggle Challenege



## Citations

* https://www.kaggle.com/competitions/nyc-taxi-trip-duration
* https://www.kaggle.com/code/sudhirnl7/linear-regression-tutorial
* https://www.askpython.com/python/examples/rmse-root-mean-square-error
* https://www.kaggle.com/code/salvarezgonz/nyc-taxi-duration-regression-lightgbm-ml-model






