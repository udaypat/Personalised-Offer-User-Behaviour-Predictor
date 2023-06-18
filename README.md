# Driver Behavior Discount Preference Predictor

## Overview

This GitHub repository contains data collected through a survey aimed at understanding drivers' behavior regarding their preference for discounts/offers for dining/takeaway. The survey was conducted by providing different scenarios to various users to gather insights into their decision-making process.

You are driving from IIT Madras to Chennai Airport along with your family, and you receive an offer of a 10 percent discount on the bill from a famous Chinese restaurant in Guindy. Will you avail of the offer while travelling?

In addition to the user's response to the scenario, basic information about the users was collected for further analysis.

## Data Collection

The data in this repository was collected through an online survey platform. Participants were presented with the scenario and were asked to choose between availing or not availing the offered discount. Alongside this choice, basic demographic and user-specific information was collected to provide context for the analysis.



In addition to the user's response to the scenario, basic demographic and user-specific information was collected for further analysis.



## Data Cleaning and Analysis
The following steps were followed to clean the data and find the best parameters:

1. **Data Cleaning:**
   - Done using `numpy` and `pandas`
   - Remove any duplicate entries from the dataset, if applicable.
   - Check for missing values in the dataset.
   - Standardize the format of the data, ensuring that all relevant variables are in a consistent and comparable format.

3. **Data Pre Processing:**
   - Created a `sklearn pipeline `using `Simple Inputer`, `Standard Scaler`
   - Applied it on respective coloums using `Column Transformer`
   - Used `OneHotEncoder` and `Ordinal Encoder` for feature engineering. 

4. **Model Building and Parameter Tuning:**
   - Split the data into training and testing sets using `test_train_split`
   - Used a for loop to loop through most common classifiers.
   - Perform hyperparameter tuning to find the best set of parameters using `Grid Search CV` and `Random CV`
   - Evaluate the models using appropriate evaluation metrics, such as `accuracy`, `precision`, `recall`, or `F1 score`.




## Repository Contents

- `train_data.csv`: This CSV file contains the collected data, including user responses to the scenario and associated demographic information used for training the model.

- `test_data.csv`: Test Data For model performance

- `model.ipynb`: A Jupyter Notebook containing  analysis of the collected data. This notebook demonstrates how to load, clean, and explore the data, and provides a machine learning model to predict user behivaiour.
ts.

- `submission.csv`: Final predictions exported by ML model.