
# Data Science Task 4: Email Spam Detection with Machine Learning

## What this project does

This project builds a model that reads a text message and predicts whether it is spam or a legitimate message (ham). This is a Natural Language Processing task, meaning the input is raw text rather than numbers.

## Why this matters

This task introduces text based machine learning, which works differently from the number based projects. It teaches how to clean and prepare raw text, how to convert text into numbers a model can learn from using TF-IDF, and why standard accuracy is not the full picture when one type of mistake is more costly than another.

## Dataset

The dataset is the SMS Spam Collection dataset, commonly available on Kaggle and the UCI Machine Learning Repository.

1. Go to kaggle.com and log into your account
2. Search for "SMS Spam Collection dataset"
3. Download the CSV file, often named `spam.csv`
4. When running the notebook in Colab, the upload cell near the top will show an upload button, use it to upload this file

## Tools used

1. Python
2. pandas, for handling the data as a table
3. NLTK, for text preprocessing (stopword removal and tokenization)
4. scikit learn, for TF-IDF, the classifiers, and evaluation tools
5. wordcloud, for the bonus visualizations
6. Google Colab, as the notebook environment

## What the notebook does, step by step

1. Loads the SMS dataset (uploaded by hand into Colab) and cleans up its columns
2. Checks the class distribution (how many spam vs ham messages), since this dataset is imbalanced
3. Cleans the text: lowercases it, removes punctuation, splits it into words, and removes common stopwords
4. Converts the cleaned text into numbers using TF-IDF
5. Splits the data into a training set (80 percent) and a testing set (20 percent), keeping the same spam to ham ratio in both
6. Trains two classifiers: Multinomial Naive Bayes (the industry standard for text) and Logistic Regression
7. Evaluates both models using accuracy, precision, recall, F1 score, and a confusion matrix
8. Explains why recall matters more than plain accuracy for spam detection
9. Bonus: draws word clouds showing the most common words in spam messages versus ham messages


## How to run this project

1. Download `spam.csv` from Kaggle first (see Dataset section above)
2. Open the notebook in Google Colab
3. Run the cells from top to bottom, in order (Runtime, then Run all will pause automatically at the upload cell)
4. When prompted, upload `spam.csv`
5. The first code cell downloads a couple of small NLTK resources automatically, this only needs an internet connection, no manual setup
6. Read the explanations above each code cell to understand what it is doing
7. Check the printed evaluation numbers, the confusion matrices, and the word clouds near the bottom

## Files in this folder

1. `Email_Spam_Detection.ipynb`, the full notebook with code and explanations
2. `README.md`, this file
   
