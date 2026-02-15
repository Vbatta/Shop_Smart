# 🛒 Shop Smart E-commerce Revenue Prediction
## Project Overview

This project focuses on predicting whether a user will generate revenue (purchase) on an e-commerce website using machine learning.
A Decision Tree Classifier is used after performing data preprocessing, feature engineering, exploratory data analysis (EDA), and model tuning.

The goal is to help businesses understand customer behavior and improve conversion rates.

## Problem Statement

Predict the Revenue (True/False) of a visitor based on:

- Browsing behavior

- Page duration

- Traffic type

- Visitor type

- Month & weekend activity

This is a supervised classification problem.

## Dataset

Dataset used: shop_smart_ecommerce.csv

It contains features like:

- Administrative & Administrative Duration

- Informational & Informational Duration

- ProductRelated & ProductRelated Duration

- TrafficType

- VisitorType

- Month

- Weekend

- SpecialDay

- Revenue (Target Variable)

## Technologies Used

- Python

- Pandas

- NumPy

- Matplotlib

- Seaborn

- Scikit-learn

## Project Workflow
1️⃣ Data Loading

- Loaded dataset using Pandas

- Checked basic structure and features

2️⃣ Data Preprocessing

- Label Encoding for Weekend

- One-Hot Encoding for:

  - VisitorType

  - Month

- Feature & Target split:

  - X → Features

  - y → Revenue

3️⃣ Exploratory Data Analysis (EDA)

Performed visual analysis using:

- Line plots (Duration vs Activity)

- Bar plots (Month vs Special Day)

- Traffic & Visitor behavior analysis

## Model Used
### Decision Tree Classifier

- Trained using sklearn.tree.DecisionTreeClassifier

- Train-Test Split: 55% test size

- Hyperparameter tuning performed on:

  - max_depth

  - min_samples_split

  - ccp_alpha (Cost Complexity Pruning)

## Model Tuning

The model was optimized by:

- Testing multiple tree depths (2–10)

- Adjusting minimum sample splits

- Applying Cost Complexity Pruning to reduce overfitting.

## Evaluation Metrics

- Accuracy Score - 0.901209

- F1 Score - 0.571161

F1 Score is used to handle class imbalance effectively.

## Model Visualization

The decision tree was visualized using:

plot_tree(model, feature_names=X.columns, filled=True)

This helps in understanding how the model makes decisions.
