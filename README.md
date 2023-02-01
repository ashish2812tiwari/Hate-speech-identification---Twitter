# Hate-speech-identification---Twitter
# Overview

This project aims to identify **hate speech** using *machine learning binary classification algorithms*.
Baseline models included Random Forest, Naive Bayes, Logistic Regression. The final model was a *Logistic Regression* model that used TD-IDF for feature engineering.
It produced an F1 score of 0.75 and Recall of 0.77. Therefore, our goal is to automate hate speech identification, which is a very challenging issue. And while this effort was able to start that process, more work needs to be done to prevent this content from appearing on public venues like Twitter.

**$\color{red}{\text{Warning}}$ : This notebook contains offensive language from the dataset.**

# Data & Methods

The dataset for this capstone project was obtained from Twitter using the snscrape library, which also formatted the raw data for simple understanding. $\color{red}{\text{Here we are taking only past 10000 tweets from date 31/1/2023}}$

Since content moderation is so arbitrary, this dataset's labels were chosen by a public vote and based on majority-rules. Each tweet is assigned a class—0 for hate speech, 1 for foul language, or 2 for neither—in the "class" column. I'll be handling the data as a binary classification challenge in order to develop a distinct project and modify it for my own business environment.

Therefore, the final model will be **predicting whether a tweet is hate speech or not.** In order to prepare the data for this, I will manually replace the existing values of 1 and 2 with 0 and 1 to represent hate speech.
