## NYC Bus Delay Analysis with Weather Impact
 ## Overview

This project analyzes public transportation delays in New York City and examines how weather conditions and time-based factors influence severe bus delays. The goal is to build a realistic, interpretable machine learning model using real-world data.

##  Datasets Used

NYC Bus Breakdown and Delays (NYC Open Data)

NYC Weather Data (2016–2022)

Both datasets were merged using nearest timestamps to align transit events with corresponding weather conditions.

##  Key Steps

Data cleaning and preprocessing of noisy real-world datasets

Handling extreme outliers in delay duration

Feature engineering (peak hours, weekend flags, weather indicators)

Exploratory Data Analysis (EDA) to identify delay patterns

Predictive modeling using Logistic Regression, Decision Tree, and Random Forest

Model validation using train-test split, confusion matrix, ROC curve, and learning curves

## Model & Results

Final Model: Random Forest Classifier

## Test Accuracy: ~79%

Demonstrated strong generalization with minimal train–test performance gap

No evidence of overfitting based on learning curve analysis

## Key Insights

Peak hours and rainy conditions significantly increase delay risk

Severe delays are harder to predict due to operational randomness

Tree-based models outperform linear baselines for this problem

## Tech Stack

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

 ## Future Improvements

Incorporate route-level historical trends

Add traffic or GPS-based features

Deploy model as a simple API or dashboard
