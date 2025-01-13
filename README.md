# 2024 U.S. Election Sentiment Analysis on X (Twitter)

This project focuses on sentiment analysis of tweets related to the 2024 U.S. Election using a fine-tuned RoBERTa model. The goal is to classify tweets into three sentiment categories: **positive**, **neutral**, and **negative**.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Model Training](#model-training)
6. [Results](#results)
7. [Inference](#inference)
8. [License](#license)

---

## Project Overview

The project involves:
- Preprocessing tweet data related to the 2024 U.S. Election.
- Fine-tuning a **RoBERTa-base** model for sentiment classification.
- Evaluating the model's performance on a test dataset.
- Saving the fine-tuned model for future use.
- Performing inference on new tweets to predict sentiment.

The model achieved **100% accuracy** on the test set, demonstrating strong performance in classifying tweet sentiments.

---

## Dataset

The dataset consists of tweets related to the 2024 U.S. Election, labeled with one of three sentiments:
- **Positive**
- **Neutral**
- **Negative**

The dataset is split into three files:
- `train.csv`: Training data
- `val.csv`: Validation data
- `test.csv`: Test data

Each row in the dataset contains:
- `tweet_id`: Unique identifier for the tweet
- `user_handle`: Twitter handle of the user
- `timestamp`: Time when the tweet was posted
- `tweet_text`: Text content of the tweet
- `candidate`: Candidate mentioned in the tweet
- `party`: Political party of the candidate
- `retweets`: Number of retweets
- `likes`: Number of likes
- `sentiment`: Sentiment label (positive, neutral, negative)

---
