# 2024 U.S. Election Sentiment Analysis on X (Twitter)

This project focuses on sentiment analysis of tweets related to the 2024 U.S. Election using a fine-tuned RoBERTa model. The goal is to classify tweets into three sentiment categories: **positive**, **neutral**, and **negative**.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Results](#results)
4. [Inference](#inference)
5. [License](#license)

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

## Results

The fine-tuned RoBERTa model achieved **100% accuracy** on the test set. Here is the classification report:

          precision    recall  f1-score   support
negative       1.00      1.00      1.00         3
 neutral       1.00      1.00      1.00        13
positive       1.00      1.00      1.00        34
accuracy                           1.00        50

---

## Inference

The fine-tuned model can be used to predict sentiment on new tweets. For example, given the tweet:

> "Kamala Harris's new policy on education reform is impressive."

The model predicts the sentiment as **positive** with a confidence score of **0.997**.

---


## Acknowledgments
- [Hugging Face](https://huggingface.co/) for the `transformers` library.
- [RoBERTa](https://arxiv.org/abs/1907.11692) for the base model.
