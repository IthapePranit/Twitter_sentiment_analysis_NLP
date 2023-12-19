# Twitter_sentiment_analysis_NLP

## Overview

This project involves sentiment analysis on Twitter data using natural language processing (NLP) techniques and machine learning. The goal is to classify tweets into different sentiment categories (Positive, Negative, Neutral) based on their content.

## Project Highlights

- **Data Cleaning and Preprocessing:** Utilized Pandas for data cleaning, dropping unnecessary columns, and handling missing values. Applied various text cleaning techniques, such as lowercasing, URL removal, HTML tag removal, punctuation removal, and emoji conversion.

- **Feature Engineering:** Created new features such as character length, word count, average word length, stop words count, hashtag count, mention count, and digit count to enhance the model's understanding of the data.

- **Data Visualization:** Employed Matplotlib and Seaborn for visualizing sentiment distribution and exploring numerical features. Generated word clouds to visually represent the most common words in each sentiment category.

- **Machine Learning Model:** Developed a sentiment classification model using a pipeline that includes TF-IDF Vectorization and a Random Forest Classifier. Achieved an impressive test accuracy of 94%.

## Project Structure

The project is organized as follows:

- **Data:** Contains the dataset used for training and testing the model (`twitter_training.csv`).

- **Notebooks:** Jupyter Notebooks used for data exploration, feature engineering, model development, and data visualization.

- **Scripts:** Python scripts for specific tasks, such as text cleaning (`text_cleaning.py`).

- **Requirements:**
import pandas as pd
import re
import string
import nltk
from nltk.corpus import stopwords
from sklearn.model_selection import train_test_split
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.ensemble import RandomForestClassifier
from sklearn.pipeline import Pipeline
from sklearn.metrics import classification_report
from wordcloud import WordCloud, STOPWORDS
import matplotlib.pyplot as plt
import seaborn as sns
from bs4 import BeautifulSoup
import emoji

## Getting Started

1. Clone the repository: `git clone [repository_url]`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Explore the Jupyter Notebooks in the "Notebooks" directory for a detailed walkthrough.

## Model Evaluation

The machine learning model achieved the following results:

- **Precision:** 93%
- **Recall:** 92%
- **F1-Score:** 92%
- **Test Accuracy:** 94%

## Conclusion

This project showcases skills in natural language processing, data preprocessing, feature engineering, data visualization, and machine learning. The sentiment analysis model demonstrates effectiveness in classifying tweets based on sentiment.

