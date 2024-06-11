# Module 13 Challenge - Spam Detector

## Background
The assignment assumes that you work at an Internet Service Provider (ISP) and you've been tasked with improving the email filtering system for its customers. You've been provided with a dataset that contains information about emails, with two possible classifications: spam and not spam. The ISP wants you to take this dataset and develop a supervised machine learning (ML) model that will accurately detect spam emails so it can filter them out of its customers' inboxes. The program will be creating two classification models to fit the provided data, and evaluate which model is more accurate at detecting spam. The models will be a logistic regression model and a random forest model.

## Code Source
The code location is: [Click Here to view](https://github.com/jaidevkler/classification-challenge)

## Files
spam_detector.ipynb [Click here to view](https://github.com/jaidevkler/classification-challenge/blob/main/spam_detector.ipynb)

## How to run the program
Download the files and then use jupyter notebook or jupyter lab to open the Crypto_Clustering_starter_code.ipynb file.<br />

## Predictions
The Random forest will outperform as it is a powerful machine-learning technique that has the potential to yield better results than logistic regression. It is an ensemble of decision trees, which are much more powerful at capturing non-linear relationships between features and target variables.

## Activity

### 1. Split the Data into Training and Testing Sets
* Read the data from https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv Links to an external site. into a Pandas DataFrame.
* In the appropriate markdown cell, make a prediction as to which model you expect to do better.
* Create the labels set (y) from the “spam” column, and then create the features (X) DataFrame from the remaining columns.
* Check the balance of the labels variable (y) by using the value_counts function.
* Split the data into training and testing datasets by using train_test_split.

### 2. Scale the Features
* Create an instance of StandardScaler.
* Fit the Standard Scaler with the training data.
* Scale the training and testing features DataFrames using the transform function.

### 3. Create a Logistic Regression Model
* Fit a logistic regression model by using the scaled training data (X_train_scaled and y_train). Set the random_state argument to 1.
* Save the predictions on the testing data labels by using the testing feature data (X_test_scaled) and the fitted model.
* Evaluate the model’s performance by calculating the accuracy score of the model.

### Create a Random Forest Model
* Fit a random forest classifier model by using the scaled training data (X_train_scaled and y_train).
* Save the predictions on the testing data labels by using the testing feature data (X_test_scaled) and the fitted model.
* Evaluate the model’s performance by calculating the accuracy score of the model.

### 4. Evaluate the Models
* Which model performed better? The Random Forrest model performed better than the Logistic Regression model, as the accuracy score of the y_test vs predictions was higher: 96.6% for Random Forrest Model vs 92.8% for Logistic Regression Model.
* How does that compare to your prediction? The results were inline with the predictions at the start.


## Reference
Columbia AI Bootcamp - Module 13 Challenge<br />
Data: https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv

