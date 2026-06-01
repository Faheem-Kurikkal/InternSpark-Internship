# InternSpark-Internship
This repository is made for my submission of Tasks/projects under InternSpark internship


# Task 1 : Iris Classification


## Project Description

### Objective:

Predict iris flower species using machine learning.

This project classifies Iris flowers into three species:
- Setosa
- Versicolor
- Virginica

The dataset used is the Iris Classification Dataset from Kaggle.

## Algorithms Used
1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Decision Tree

The best-performing model was saved as 'iris_model.pkl'.

## Running the Notebook

Open and run: 

Iris_Classification.ipynb

## Inference Example

## Python:

import pandas as pd
import joblib

model = joblib.load('iris_model.pkl')

scaler = joblib.load('scaler.pkl')

sample = [[5.1,3.5,1.4,0.2]]

sample = scaler.transform(sample)

prediction = model.predict(sample)

print("Predicted Species: ", encoder.inverse_transform(prediction)[0])


## Expected Output:
Iris-versicolor.
