# Recipe Rating Prediction 🍽️📊

## Overview

This project focuses on predicting user ratings for recipes using structured review data and user interaction signals. The goal is to demonstrate how data preprocessing, exploratory data analysis, and machine learning models can be used to extract insights from real-world datasets and make reliable predictions.

The project covers the complete data science lifecycle—from raw data to model evaluation—making it a strong example of applied data analysis and predictive modeling.

---

## Problem Statement

Online recipe platforms rely heavily on user ratings to recommend content and surface high-quality recipes. However, ratings are influenced by multiple factors such as:

- User reputation  
- Engagement signals (thumbs up / thumbs down)  
- Review characteristics  
- Temporal patterns  

This project aims to predict recipe ratings using these features, enabling platforms to better understand user behavior and improve recommendation quality.

---

## Dataset

- Dataset size: 18,000+ records  
- Total features: 15  
- Key attributes include:
  - User reputation
  - Thumbs up / thumbs down counts
  - Review text
  - Timestamps
  - Star ratings (target variable)

The dataset includes numerical, categorical, textual, and temporal features suitable for both exploratory analysis and predictive modeling.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Handling missing values through imputation
- Removing duplicate records
- Identifying and treating outliers
- Converting UNIX timestamps into readable datetime formats

### Feature Engineering
- Extracted Year, Month, Day, and Hour from timestamps
- Created derived numerical features
- Prepared categorical variables for statistical analysis

---

## Exploratory Data Analysis (EDA)

EDA was conducted to understand patterns, trends, and relationships within the data:

- Distribution analysis of numerical features
- Rating frequency analysis using count plots and pie charts
- Pairwise feature analysis using scatter and pair plots
- Review length analysis
- Correlation analysis using heatmaps
- Multicollinearity detection using Variance Inflation Factor (VIF)
- Chi-square tests for categorical feature significance

Insights from EDA guided feature selection and model choice.

---

## Machine Learning Models

The following classification models were implemented and compared:

- Logistic Regression
- Decision Tree Classifier
- XGBoost
- LightGBM (LGBM)

### Model Optimization
- Hyperparameter tuning using GridSearchCV
- Cross-validation for performance stability

---

## Model Evaluation

Models were evaluated using:

- Accuracy
- Precision, Recall, and F1-score
- Confusion Matrix
- ROC Curves (One-vs-Rest)
- Learning Curves
- Comparative performance analysis

### Final Model Selection
XGBoost achieved the best overall performance and was selected as the final model for prediction.

---

## Tech Stack

- Programming Language: Python
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - XGBoost
  - LightGBM

---

## Project Structure

├── recipe-rating-prediction.ipynb
├── data/
│ └── dataset.csv
├── outputs/
│ └── predictions.csv
├── README.md


---

## Key Takeaways

- Demonstrates strong data cleaning and preprocessing skills
- Covers complete end-to-end machine learning workflow
- Emphasizes model evaluation and comparison
- Focuses on explainability and data-driven insights

---

## Future Enhancements

- Integrate NLP techniques for review text analysis
- Explore deep learning models
- Perform advanced feature selection
- Deploy the model as an API for real-time predictions
