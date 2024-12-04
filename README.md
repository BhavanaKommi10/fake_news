# Fake News Detection Model
This project implements a machine learning-based fake news detection model, capable of classifying news articles as either "Real" or "Fake" based on their content. The model uses several classifiers to determine accuracy and classify news based on provided input text.

## Table of Contents
#### 1. Dataset Loading and Preparation
#### 2. Data Preprocessing
#### 3. Data Splitting and Vectorization
#### 4. Model Training and Evaluation
#### 5. Testing with Manual Input
#### 6. Function Documentation


### 1. Data Collection
The datasets True.csv and Fake.csv are loaded from Google Drive. They contain labeled examples of true and fake news articles, respectively. A label column is added to identify real news with a 1 and fake news with a 0.

### 2. Data Preprocessing
Unnecessary columns are removed, and text data is cleaned using a custom function wordopt, which:
#### Converts text to lowercase
#### Removes HTML tags, URLs, punctuation, numbers, and extra whitespace

### 3. Data Splitting and Vectorization
The data is split into training and test sets.

### 4. Model Training and Evaluation
Three classifiers are trained:
#### Logistic Regression
#### Decision Tree
#### Random Forest
Each classifier is evaluated on accuracy, precision, recall, and F1-score

### 5. Manual Output
A manual testing function takes a news article as input, applies preprocessing, and uses each classifier to predict whether the news is real or fake.

### 6. Function Documentation
#### wordopt(text): Cleans the input text by removing HTML tags, URLs, punctuation, numbers, and converting to lowercase.
#### output(n): Returns "Real News" if input is 1, "Fake News" if input is 0.
#### manual_testing(news): Takes a raw news article, cleans it, vectorizes, and returns predictions from each model.
