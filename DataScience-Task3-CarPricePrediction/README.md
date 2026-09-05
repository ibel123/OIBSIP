# Data Science Task 3: Car Price Prediction with Machine Learning

## What this project does

This project builds a model that predicts the selling price of a used car based on details like its brand, age, mileage, fuel type, and transmission type.

## Why this matters

Real datasets almost never come clean and ready to use. This project focuses heavily on cleaning: fixing inconsistent text, handling missing values, removing duplicates, and creating new useful features out of raw columns. Cleaning well is often more important to a project's success than which model you choose at the end.

## Dataset

The dataset is a used car listings dataset, commonly called the "Vehicle dataset from cardekho" on Kaggle.

1. Go to kaggle.com and log into your account
2. Search for "Vehicle dataset from cardekho" or "Car Price Prediction dataset"
3. Download the CSV file
4. When running the notebook in Colab, the upload cell near the top will show an upload button, use it to upload this file

## Tools used

1. Python
2. pandas and numpy, for handling and cleaning the data
3. matplotlib and seaborn, for charts
4. scikit learn, for the regression models and evaluation tools
5. Google Colab, as the notebook environment

## What the notebook does, step by step

1. Loads the car dataset (uploaded by hand into Colab)
2. Checks the shape, data types, missing values, and duplicate rows
3. Cleans the data: removes duplicates, fills missing values, standardizes inconsistent text (like "Petrol" vs "petrol")
4. Engineers two new features: car age (from the year) and brand (extracted from the car name)
5. Explores the cleaned data with histograms, box plots, and scatter plots
6. Groups rare brands into an "other" category, then one hot encodes all categorical columns
7. Builds a correlation heatmap
8. Splits the data into a training set (80 percent) and a testing set (20 percent)
9. Trains two models: Linear Regression (baseline) and Random Forest Regressor (comparison)
10. Evaluates both models using MAE, RMSE, and R squared
11. Looks at which features the Random Forest model relied on most

## How to run this project

1. Download the car dataset from Kaggle first (see Dataset section above)
2. Open the notebook in Google Colab
3. Run the cells from top to bottom, in order (Runtime, then Run all will pause automatically at the upload cell)
4. When prompted, upload your CSV file
5. Check the printed column names against the code, if anything does not match, adjust the column names in the code cells that follow
6. Read the explanations above each code cell to understand what it is doing
7. Check the printed evaluation numbers and the feature importance chart near the bottom

## Files in this folder

1. `Car_Price_Prediction.ipynb`, the full notebook with code and explanations
2. `README.md`, this file
3. `car data.csv/`

