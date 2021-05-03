# Rain-in-Australia---ML-Classification
This project analyze ML Model performance and methods to deal with class imbalance.

# Steps of Project
1: Preprocessing and visualize data.\
2: Apply over-sampling, under sampling and hybrid techniques to deal with class imbalance.\
3: Apply ML Models to treated train data. Monitor Performance.

# Data Source/Brief
https://www.kaggle.com/jsphyg/weather-dataset-rattle-package \
23 Columns,145461 rows. Both continuous and discrete variables.\
Dependent variable: Rain Next Day 1 or 0. \
Independent variable: Windspeed, Humidity, MaxTemperature, MinTemperature, Pressure, Sunshine etc.

# Data Preprocessing
1: Identify and fill missing values (median and mode fill)\
2: Visualize class distribution (20% - Rain and 80% - No Rain), Correlation (heatmap) and independent variable distributions\
3: Removing Outliers\
4: 20% 80% Train Test Split

# Treatment on Train Data
1: Original Data (untreated)\
2: SMOTE (oversampling)\
3: SMOTE + TomekLinks (hybrid)\
4: SMOTE + ENN (hybrid)

# ML Models
Four different Models are run on each of the train data.\
1: Logistic Regression \
2: Naive Bayes \
3: Random Forest \
4: XGBoost 

# Performance Metrics
1: f1 score\
2: Accuracy, Precision, Recall\
3: ROC AUC

# Conclusion:
- Oversampling or undersampling significantly improved Recall at the cost of worse Precision
- Overall performance did not increase significantly.
- Random Forest Model with 1000 trees performs best in general. XGBoost is extremely close. Naive Bayes performs worst.
- Sampling techniques may have bigger benefit when applied to more extreme cases of class imbalance. 


