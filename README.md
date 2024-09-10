# Click-Through Rate (CTR) Analysis and Prediction

This project analyzes and predicts click-through rates (CTR) based on user behavior data. The dataset used includes various features such as daily time spent on a website, age, income, and more. The goal is to predict whether a user will click on an advertisement using machine learning models.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Description](#data-description)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Data Preprocessing](#data-preprocessing)
- [Modeling and Evaluation](#modeling-and-evaluation)
- [Results](#results)

## Project Overview

This project involves the following steps:

1. **Data Exploration**: Initial exploration to understand the data distribution and relationships between features.
2. **Feature Engineering**: Creating new features and categorizing continuous features into discrete buckets.
3. **Data Preprocessing**: Handling missing values, scaling numerical features, and encoding categorical features.
4. **Model Training**: Building a Random Forest classifier to predict whether a user will click on an ad.
5. **Evaluation**: Assessing model performance using accuracy and classification metrics.

## Data Description

The dataset consists of 10,000 records with the following key features:

- `Daily Time Spent on Site`: Time (in minutes) spent on the site.
- `Age`: User's age.
- `Area Income`: Average income of the user's geographical area.
- `Daily Internet Usage`: Time (in minutes) spent on the internet.
- `Clicked on Ad`: Binary target variable indicating whether the ad was clicked (1) or not (0).

## Exploratory Data Analysis

Several visualizations were created to explore the relationships between the features and the target variable (`Clicked on Ad`). Key insights include:

- **Daily Time Spent on Site**: Users who clicked on ads tend to spend more time on the site.
- **Daily Internet Usage**: Higher internet usage correlates with a higher likelihood of clicking on ads.
- **Age and Income**: Age and income are also explored to understand their influence on CTR.

## Feature Engineering

Custom buckets were created for the following features:

- **Daily Time Spent on Site**: Categorized into `Low`, `Medium`, `High`, and `Very High`.
- **Age**: Categorized into `Below 18`, `18-25`, `26-35`, `36-45`, and `46+`.
- **Area Income**: Categorized into `Very Low`, `Low`, `Medium`, and `High`.

These engineered features help in better capturing the relationships within the data.

## Data Preprocessing

A preprocessing pipeline was set up to:

- **Numerical Features**: Impute missing values with the median and scale the data.
- **Categorical Features**: Impute missing values with the most frequent category and apply one-hot encoding.

## Modeling and Evaluation

A **Random Forest** classifier was used to model the data. The pipeline for the model included:

1. **Data Type Conversion**: Ensure all features are in the correct format.
2. **Feature Engineering**: Apply the custom buckets for `Daily Time Spent on Site`, `Age`, and `Income`.
3. **Preprocessing**: Impute and scale/encode features.
4. **Classification**: Train the model and evaluate its performance.

### Results

The model was evaluated using accuracy and a classification report, which includes precision, recall, and F1-score.

- **Accuracy**: The proportion of correctly classified instances.
- **Classification Report**: Detailed metrics for each class.


