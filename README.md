# Data-Mining-Kaggle-Competition

**Political View Classification from Tweets**

This project involved building a machine learning model to classify the political orientation of European politicians based solely on their tweets. The goal was to infer whether a politician leans left, center, or right using natural language processing techniques.

**Overview**

Task: Multiclass classification (left, center, right)

Input: Tweet text from European politicians

Output: Predicted political stance

Model Used: Logistic Regression

Final Accuracy: 78%

Leaderboard Placement: 6th / ~50 teams

**Project Structure**

├── README.md

├── kaggle_project.ipynb     # Notebook with EDA and final model + submission

├── model.ipynb              # Notebook with training and evaluation of different models

└── lemmatizer.py            # Script for lemmatizing tweets


**Approach**

Data Preprocessing:
  - Tokenization & lowercasing
  - Removal of URLs, mentions, and punctuation
  - Stopword removal
  - TF-IDF vectorization of tweets

Modeling: Logistic Regression

**Requirements**

Python 3.8+

scikit-learn

pandas

matplotlib

seaborn

nltk

**Key Learnings**

TF-IDF combined with Logistic Regression is surprisingly effective for political text classification and outperformed my attempts at SVM, Random Forest, and Neural Networks.
Preprocessing choices (like setting the n-grams in the TF-IDF vectorizer) can have a significant impact on model performance.
