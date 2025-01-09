# Anomaly-Detection-Capstone
# Automated Anomaly Detection for Predictive Maintenance
**Author**: Debangana Chatterjee

**Course**: Data Science Bootcamp,upGrad

## Contents
1. [Introduction](#introduction)
2. [Dataset Overview](#dataset-overview)
3. [Design Choices](#design-choices)
4. [Data Preprocessing](##data-preprocessing)
5. [Feature Engineering](##feature-engineering)
6. [Model Selection and Training](##model-selection-and-training)
7. [Model Validation](##model-validation)
8. [Performance Evaluation](#performance-evaluation)
9. [Future Work](#future-work)
10. [Source Code](#source-code)
11. [Conclusion](#conclusion)

---

## Introduction
Many industries need predictive maintenance solutions to reduce risks and gain actionable insights by processing data from their equipment. This project aims to predict machine breakdowns by identifying anomalies in the data.

Predictive maintenance evaluates equipment conditions through online monitoring to perform maintenance before equipment degrades or breaks down.

---

## Dataset Overview
This project focuses on developing an automated anomaly detection system for predictive maintenance using time-series data. The dataset consists of over 18,000 rows, with a binary column (`y`) indicating anomalies (1 for anomaly, 0 for normal operation). The remaining columns are predictors.

---

## Design Choices
- **Data Preprocessing:**
  - Handled missing values and verified feature data types.
  - Addressed class imbalance using outlier removal and oversampling.
  - Standardized features with `StandardScaler`.

- **Feature Engineering:**
  - Visualized feature correlation plots.
  - Derived metrics (sum, mean, std, min, max) to capture trends.
  - Added new time-related features (`hour`, `month`, `date`).
  - Used feature importance analysis from XGBoost and Random Forest.

- **Model Selection and Training:**
  - Models used: Logistic Regression, Random Forest, SVM, Gradient Boosting (XGBoost).
  - Split data into training, validation, and test sets.
  - Tuned hyperparameters to optimize model performance.

---

## Model Validation
Performance was evaluated using metrics like:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix

---

## Performance Evaluation
- Accuracy exceeded 75%, meeting success criteria.
- AUC scores for models: 0.99–1.00.
- Random Forest and XGBoost highlighted significant feature predictors.

---

## Future Work
- Implement deep learning techniques like LSTMs for time-series forecasting.
- Include external factors such as weather data or operational logs.
- Develop a system for continuous monitoring and model adaptation.

---

## Source Code
The project steps include:
1. Data Loading and Cleaning
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Model Training and Evaluation
5. Saving the Model for Deployment

---

## Conclusion
This project successfully implemented an anomaly detection pipeline for predictive maintenance. The results validate its effectiveness, and proposed enhancements provide a roadmap for future optimization and deployment.
