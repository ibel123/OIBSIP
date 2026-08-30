# Data Science Task 2: Sales Prediction Using Python

## What this project does

This project builds a model that predicts product sales based on how much money is spent on advertising across three channels: TV, Radio, and Newspaper.

## Why this matters

This is a classic regression problem. Instead of predicting a category, we are predicting a number, the amount of Sales. It also teaches how to interpret a model, not just measure its accuracy, since the point of this project is to figure out which advertising channel is worth investing in.

## Dataset

The dataset is called `Advertising.csv`. It is not built into any Python library, so it needs to be downloaded from Kaggle and uploaded into the notebook.

1. Go to kaggle.com and log into your account
2. Search for "Advertising dataset" or "Advertising.csv"
3. Download the CSV file
4. When running the notebook in Colab, the second code cell will show an upload button, use it to upload this file

## Tools used

1. Python
2. pandas, for handling the data as a table
3. matplotlib and seaborn, for charts
4. scikit learn, for the regression models and evaluation tools
5. Google Colab, as the notebook environment

## What the notebook does, step by step

1. Loads the Advertising dataset (uploaded by hand into Colab)
2. Checks the shape, confirms there are no missing values, and looks at descriptive statistics
3. Draws a pairplot and individual scatter plots of each channel against Sales
4. Builds a correlation heatmap to see which channel relates most strongly to Sales
5. Splits the data into a training set (80 percent) and a testing set (20 percent)
6. Trains a baseline Linear Regression model
7. Trains a second model, Random Forest Regressor, for comparison
8. Evaluates both models using MAE, RMSE, and R squared
9. Draws a residual plot to check whether the Linear Regression model is missing any pattern
10. Looks at the Linear Regression coefficients and Random Forest feature importances to work out which channel matters most

## Results

Both models typically achieve a high R squared score on this dataset, since sales are strongly driven by advertising spend. TV spend usually turns out to be the strongest driver of Sales, followed by Radio, with Newspaper spend having very little measurable effect.

## How to run this project

1. Download `Advertising.csv` from Kaggle first (see Dataset section above)
2. Open the notebook in Google Colab
3. Run the cells from top to bottom, in order (Runtime, then Run all will pause automatically at the upload cell)
4. When prompted, upload `Advertising.csv`
5. Read the explanations above each code cell to understand what it is doing
6. Check the printed evaluation numbers and the coefficient and feature importance tables near the bottom

## Files in this folder

1. `Sales_Prediction.ipynb`, the full notebook with code, visuals and explanations
2. `README.md`, this file


