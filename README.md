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
├── tweets_political_classifier.ipynb     # Main notebook with training, evaluation, and submission
├── train.csv                             # Provided training data
├── test.csv                              # Provided test data (no labels)
├── submission.csv                        # Final predictions for Kaggle submission
├── requirements.txt                      # Project dependencies
└── plots/
    └── confusion_matrix.png              # Model performance visualization

**Approach**

Data Preprocessing:
  Tokenization & lowercasing
  Removal of URLs, mentions, and punctuation
  Stopword removal (optional)
  TF-IDF vectorization of tweets
Modeling
Multinomial Logistic Regression
Used stratified train/validation split for tuning
Evaluated using accuracy and confusion matrix
Submission
Trained on full data
Generated predictions on test set for Kaggle submission
📊 Results

Metric	Value
Accuracy	78%
Rank	6/50
The model performed especially well in distinguishing between left and right, with occasional confusion in identifying centrist tweets.

🛠 Requirements

Python 3.8+
scikit-learn
pandas
matplotlib
seaborn
nltk
Install requirements with:

pip install -r requirements.txt
🧠 Key Learnings

TF-IDF combined with Logistic Regression is surprisingly effective for political text classification.
Language used by politicians differs strongly by ideology, even across countries.
Preprocessing choices (like whether to keep stopwords) can have a significant impact on model performance.
