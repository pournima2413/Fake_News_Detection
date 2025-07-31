# Fake_News_Detection
## Overview 
This project aims to build a machine learning-based system to detect whether a news article is fake or real. With the growing spread of misinformation online, fake news detection has become a crucial application of Natural Language Processing (NLP) and machine learning.
We use text preprocessing, TF-IDF vectorization, and multiple classification algorithms to accurately classify news content. Manual testing is also included for real-world simulation.

## Dataset
1. Fake.csv
2. True.csv  // Source: Kaggle Open Data Repositories

## Project WorkFlow
1. Data Loading: Loaded both Fake.csv and True.csv using Pandas.
2. Data Labelling : Added class labels and removed the last 10 rows from each dataset for manual testing.
3. Data Cleaning : Proform Data Cleaning 
4. Merging Dataset : Combined the datasets and removed irrelevant columns (title, subject, date).
5. Dropping Unnecessary Columns
6. Text Preprocessing :
    Applied custom cleaning function using regex to:
    -- Convert to lowercase
    -- Remove punctuation, numbers, URLs, and special characters
7. Splitting Features and Labels: Split the data (75% training, 25% testing) using train_test_split.
8. Train-Test Split
9. TF-IDF Vectorization : Used TfidfVectorizer to convert text into numerical features.
10. Model Training and Classification:
    Trained all four models on the TF-IDF-transformed data and evaluated them using:
      -- Accuracy Score
      -- Classification Report (Precision, Recall, F1-score)
11. Models Used
    a. Logistic Regression
    b. Decision Tree
    c. Gradient Boosting
    d. Random Forest
