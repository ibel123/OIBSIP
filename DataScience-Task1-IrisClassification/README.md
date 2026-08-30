# Data Science Task 1: Iris Flower Classification

## What this project does

This project trains a machine learning model that looks at the physical measurements of an iris flower (sepal length, sepal width, petal length, petal width) and predicts which of three species it belongs to: Setosa, Versicolor, or Virginica.

## Why this matters

This is a classic starting project in machine learning because the dataset is small, clean, and easy to understand. It teaches the full workflow used in almost every classification task: loading data, exploring it, visualizing it, training a model, and checking how well that model performs.

## Dataset

The dataset is the Iris dataset, built directly into the scikit learn library. No download is needed. It contains 150 flower samples, 50 of each species.

## Tools used

1. Python
2. pandas, for handling the data as a table
3. matplotlib and seaborn, for charts
4. scikit learn, for the machine learning models and evaluation tools
5. Google Colab, as the notebook environment

## What the notebook does, step by step

1. Loads the Iris dataset and turns it into a table
2. Checks the shape, data types, and confirms there are no missing values
3. Shows descriptive statistics (average, minimum, maximum for each measurement)
4. Draws a pairplot and box plots to visually compare the three species
5. Discusses which features separate the species best
6. Splits the data into a training set (80 percent) and a testing set (20 percent)
7. Trains two different models: Logistic Regression and K Nearest Neighbors
8. Evaluates both models using accuracy, a confusion matrix, and a classification report
9. Declares the better performing model with a short explanation

## Results

Both models typically score above 95 percent accuracy on this dataset. The exact winner and its accuracy score will show up when you run the notebook, since results can shift very slightly depending on the random split. The final markdown cell in the notebook explains how to read the results and write your own conclusion.

## How to run this project

1. Open the notebook in Google Colab
2. Run every cell from top to bottom, in order (Runtime, then Run all)
3. Read the explanations above each code cell to understand what it is doing
4. Check the printed accuracy scores and confusion matrices near the bottom

## Files in this folder

1. `Iris_Classification.ipynb`, the full notebook with code and explanations
2. `README.md`, this file
3. `Live_Demo/`, folder for output of the notebook

