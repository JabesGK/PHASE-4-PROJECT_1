# **GROUP 3-PHASE 4-PROJECT**

## **Topic: Sentiment Analysis of Twitter Google and Apple products**

## Overview

This project, undertaken by Group 3 - Phase 4, explores how Natural Language Processing (NLP) can be applied to analyze public sentiment from Twitter regarding Apple and Google products. Using machine learning classifiers and text vectorization techniques, we build and evaluate models that can automatically detect whether a tweet expresses positive, negative, or neutral sentiment.

## Objective

The primary goal is to:

*Develop an NLP model that classifies Tweets about Apple and Google products into positive, negative, or neutral sentiment.*

This proof of concept supports:

Marketing and brand perception monitoring.

Customer service by surfacing common product issues.

Product teams by highlighting recurring praise or complaints.

## Project Structure

### 1. Business Understanding

We define the business case for leveraging sentiment analysis to improve product experience, brand loyalty, and customer responsiveness.

### 2. Data Understanding

The dataset was sourced from CrowdFlower and contains thousands of tweets labeled with emotions and product mentions.

### 3. Exploratory Data Analysis (EDA)

We examine class distributions, product mentions, missing values, and initial insights to guide cleaning and modeling. Notably:

Most tweets are positively skewed.

Products like iPhone have relatively higher negative sentiment.

### 4. Natural Language Processing (NLP)

We clean, tokenize, and vectorize tweet text using both unigram and n-gram TF-IDF. Various preprocessing strategies were explored to improve feature richness and model readiness.

### 5. Model Training and Evaluation

We trained and compared several classifiers:

Logistic Regression (baseline)

XGBoost (boosted trees)

We addressed class imbalance using SMOTE and applied GridSearchCV for hyperparameter tuning.

## Key Results:

Binary Classification (Positive vs Negative): F1 ~ 0.91 (Logistic Regression)

Multiclass Classification (Positive, Negative, Neutral):

F1 for positive ≈ 0.89

F1 for negative ≈ 0.20

Neutral often misclassified

## 6. Insights & Visualizations

We answered key questions:

Most sentiment is positive; iPhone draws most negative feedback.

Recurring positive themes: excitement, events, app praise.

Recurring negative themes: design issues, autocorrect, frustration.

Visual tools used: bar charts, heatmaps, confusion matrices, pie charts, and scatterplots.

## 7. Conclusion and Recommendations

## Conclusion:

Models reliably classify positive sentiment but struggle with negative/neutral due to class imbalance and linguistic overlap.

TF-IDF and tuning help marginally, but richer embeddings may offer significant improvements.

Business can leverage positive themes for campaigns and monitor negative themes for product refinement.

## Recommendations:

Apply BERT/RoBERTa for contextual understanding.

Tune class weights or use advanced resampling (ADASYN).

Extend to multi-platform sentiment (Reddit, forums).

Incorporate topic modeling (e.g., LDA) for deeper theme discovery.
