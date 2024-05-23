# Lung Capacity Prediction Model

## Introduction
Creating a model capable of predicting the lung tidal volume on the basis of factors such as Age, Gender, Height, and some specific symptoms.
### Dataset
The dataset contains information on individuals' lung size, age, height in inches, smoking condition, sex, cesarean condition, number of children, and weight
[Link to the dataset](https://www.kaggle.com/datasets/sulaimanahmed/lung-capacity-data)
## Approach
### Data Preparation
Loading the Data: it is done with the help of pandas dataframe 
Haandling Missing datas: Any missing categorical data was filled with most common data and 
the missing umerical values were filled by mean of the respective column
### Splitting the into numerical and categorical columns
By doing this we can scale the numerical data using Stndard scaler and have labelled the categorical into numerical using 
OneHotEncoder
### Combining Processed Features
The numerical and categorical features were combined into a single feature set using ColumnTransformer.
## Model Training
### Splitting the Data
The processed data was split into training and testing sets using train_test_split.
### Model Selection
A RandomForestRegressor with 1000 estimators and a random state of 42 was selected for training the model.
### Training the Model
The model was trained on the training data.
### Making Predictions
Predictions were made on the test set.
## Evaluation
### Model Performance
The model's performance was evaluated using Mean Squared Error (MSE).
## Challenges and Solutions
The missing values were handeled by filling with mean and mode values
#### feature engineering
for scaling the numerical data
## Running [pre requisite]
Ensure that the following libraries installed:
pandas
numpy
scikit-learn
