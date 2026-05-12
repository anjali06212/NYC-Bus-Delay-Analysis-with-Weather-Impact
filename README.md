# Predictive Analytics for NYC Bus Delays Using Weather & Temporal Features

## Brief Description
This project focuses on analyzing and predicting severe bus delays in New York City using real-world transportation and weather datasets. The objective was to understand how weather conditions and time-based patterns influence public transport delays and build a machine learning model capable of predicting severe delay occurrences.

The project combines NYC bus breakdown data with hourly weather records and applies data preprocessing, feature engineering, exploratory data analysis (EDA), and classification models to generate insights and predictions.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---

## Features
- Cleaned and processed large real-world datasets containing noisy values
- Merged transportation and weather datasets using nearest timestamp matching
- Performed feature engineering for time and weather-related factors
- Conducted exploratory data analysis to identify delay trends
- Built classification models to predict severe delays
- Compared Logistic Regression and Random Forest performance
- Evaluated models using confusion matrix, ROC curve, and learning curves

---

## Process
1. Imported NYC bus delay and weather datasets
2. Cleaned missing values and inconsistent records
3. Converted timestamps into usable datetime formats
4. Engineered features such as:
   - Peak hour indicator
   - Weekend flag
   - Rain condition flag
   - Hour and weekday extraction
5. Merged datasets using nearest timestamps
6. Defined severe delay classification target
7. Split dataset into training and testing sets
8. Trained Logistic Regression and Random Forest models
9. Evaluated model performance and extracted insights

---

## How You Built It
The project was built using Python in Google Colab/Jupyter Notebook. The NYC bus delay dataset and NYC weather dataset were loaded and preprocessed separately. Delay durations were cleaned and capped to reduce the impact of extreme outliers.

Feature engineering techniques were applied to create meaningful predictors related to time and weather conditions. Both datasets were then merged using timestamp-based alignment with `merge_asof()`.

Machine learning models including Logistic Regression and Random Forest were trained using Scikit-learn. Random Forest achieved the best performance with approximately 79% test accuracy. Visualization libraries such as Matplotlib and Seaborn were used to analyze trends and model behavior.

---

## What You Learned
- Handling and preprocessing noisy real-world datasets
- Feature engineering for machine learning tasks
- Time-series based dataset merging
- Building and evaluating classification models
- Understanding class imbalance challenges
- Comparing linear and tree-based machine learning models
- Extracting business insights from transportation data

---

## Future Improvements
- Add route-level and borough-level historical analysis
- Integrate live traffic or GPS-based features
- Apply advanced models such as XGBoost or LightGBM
- Improve severe delay prediction using imbalance handling techniques
- Deploy the model as an interactive dashboard or API

---

## Results
- Best Model: Random Forest Classifier
- Test Accuracy: ~79%
- Peak hours and rainy weather significantly increased delay risk
- Tree-based models outperformed linear models for this problem

---
