# Customer Churn Prediction

## Project Overview

Customer churn refers to customers discontinuing a product or service. Predicting churn is important for businesses because retaining existing customers is more cost-effective than acquiring new customers.

This project focuses on building a **Customer Churn Prediction System** using Machine Learning techniques to identify customers who are likely to leave a service. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, handling class imbalance using SMOTE, model training, evaluation, and business insights generation.

The objective of this project is to help businesses proactively identify high-risk customers and improve customer retention strategies.

---

## Problem Statement

The goal of this project is to predict whether a customer is likely to churn based on customer demographics, service usage patterns, payment behavior, and customer interaction history.

By accurately identifying at-risk customers, businesses can:

- Reduce customer churn
- Improve customer retention
- Increase customer lifetime value
- Optimize marketing and engagement strategies

---

## Dataset Description

The dataset contains customer information related to subscription services and customer behavior.

### Features

| Feature | Description |
|----------------------|------------------------------------------------|
| CustomerID | Unique customer identifier |
| Age | Age of the customer |
| Gender | Gender of the customer |
| Tenure | Number of months the customer used the service |
| Usage Frequency | Frequency of service usage |
| Support Calls | Number of customer support interactions |
| Payment Delay | Delay in customer payment |
| Subscription Type | Type of subscription plan |
| Contract Length | Duration of contract |
| Total Spend | Total amount spent by customer |
| Last Interaction | Most recent customer interaction |
| Churn | Target variable (1 = Churn, 0 = Retained) |

---

## Data Preprocessing

Several preprocessing steps were performed before model training:

- Removed missing values
- Encoded categorical variables using one-hot encoding
- Applied feature scaling using StandardScaler
- Performed feature engineering
- Split dataset into training and testing sets

---

## Exploratory Data Analysis (EDA)

EDA was performed to identify important patterns and customer behavior trends.

### Key Insights

- Customers with low usage frequency are more likely to churn
- Customers with short tenure show higher churn probability
- Frequent support calls indicate dissatisfaction
- Payment delays strongly correlate with churn

### Visualizations Used

- Churn distribution plots
- Correlation heatmaps
- Boxplots
- Feature importance charts
- Confusion matrix

---

## Handling Class Imbalance using SMOTE

The dataset contained class imbalance, which can negatively affect machine learning model performance.

To solve this issue, **SMOTE (Synthetic Minority Oversampling Technique)** was applied to the training dataset.

SMOTE generates synthetic samples for the minority class to create a balanced dataset and improve model learning.

### Benefits of SMOTE

- Improves recall and F1-score
- Reduces model bias toward majority class
- Enhances churn prediction capability

---

## Machine Learning Models Used

### K-Nearest Neighbors (KNN)

KNN predicts customer churn based on the nearest neighboring data points using distance calculations.

### Random Forest

Random Forest combines multiple decision trees to improve prediction accuracy and reduce overfitting.

### XGBoost

XGBoost is a boosting algorithm that improves prediction performance using gradient boosting techniques.

---

## Model Evaluation

The models were evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC Score
- Confusion Matrix

### Final Model Selection

The **Random Forest model** was finalized because it achieved the best balance between accuracy, precision, recall, and ROC-AUC score compared to KNN and XGBoost.

### Final Random Forest Performance

| Metric    | Score |
|------------|--------|
| Accuracy   | 84%    |
| Precision  | 82%    |
| Recall     | 78%    |
| F1-score   | 80%    |
| ROC-AUC    | 0.87   |

---

## Tools and Libraries Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

### Development Environment

- Jupyter Notebook
- VS Code

---

## Project Workflow

```text
1. Data Collection
2. Data Cleaning
3. Data Preprocessing
4. Exploratory Data Analysis
5. Feature Engineering
6. Feature Scaling
7. SMOTE Application
8. Model Training
9. Model Evaluation
10. Business Insights Generation
```

---

## Key Business Insights

### High Churn Risk Customers

Customers with:

- low usage frequency
- short subscription tenure
- frequent support calls
- payment delays

were identified as high-risk customers.

---

## Business Recommendations

### 1. Improve Customer Engagement

Provide personalized recommendations and offers to low-usage customers.

### 2. Enhance Customer Support

Improve issue resolution speed to reduce customer dissatisfaction.

### 3. Offer Retention Campaigns

Provide discounts or loyalty rewards for high-risk customers.

### 4. Encourage Long-Term Contracts

Promote annual subscription plans to improve customer retention.

---

## Business Value of the Project

This solution helps businesses:

- Predict customer churn proactively
- Improve retention strategies
- Reduce revenue loss
- Increase customer lifetime value
- Support data-driven business decisions

---

## Conclusion

This project demonstrates how machine learning techniques can be used to predict customer churn and support customer retention strategies.

By combining:

- Data preprocessing
- Exploratory data analysis
- SMOTE
- Feature scaling
- Machine learning models

the system effectively identifies customers likely to churn and provides actionable business insights.

---

## Future Improvements

Future enhancements may include:

- Hyperparameter tuning
- Deep Learning models
- Real-time churn prediction dashboards
- Model deployment using Streamlit or Flask
- Integration with CRM systems

---
