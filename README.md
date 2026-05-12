Customer Churn Prediction
Project Overview
Customer churn refers to customers discontinuing a product or service. Predicting churn is important for businesses because retaining existing customers is more cost-effective than acquiring new customers.
This project focuses on building a Customer Churn Prediction System using Machine Learning techniques to identify customers who are likely to leave a service. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, handling class imbalance using SMOTE, model training, evaluation, and business insights generation.
The objective of this project is to help businesses proactively identify high-risk customers and improve customer retention strategies.
________________________________________
Problem Statement
The goal of this project is to predict whether a customer is likely to churn based on customer demographics, service usage patterns, payment behavior, and customer interaction history.
By accurately identifying at-risk customers, businesses can:
•	Reduce customer churn 
•	Improve customer retention 
•	Increase customer lifetime value 
•	Optimize marketing and engagement strategies 
________________________________________
Dataset Description
The dataset contains customer information related to subscription services and customer behavior.
Features Used
•	CustomerID 
•	Age 
•	Gender 
•	Tenure 
•	Usage Frequency 
•	Support Calls 
•	Payment Delay 
•	Subscription Type 
•	Contract Length 
•	Total Spend 
•	Last Interaction 
•	Churn (Target Variable) 
Target Variable
•	0 → Customer Retained 
•	1 → Customer Churned 
________________________________________
Project Workflow
1. Data Preprocessing
Several preprocessing steps were performed before model training:
•	Removed missing values 
•	Encoded categorical variables 
•	Applied feature scaling using StandardScaler 
•	Performed feature engineering 
•	Split dataset into training and testing sets 
________________________________________
2. Exploratory Data Analysis (EDA)
EDA was performed to understand customer behavior and identify important churn patterns.
Key Findings
•	Customers with low usage frequency are more likely to churn 
•	Customers with short tenure have higher churn probability 
•	Frequent support calls indicate customer dissatisfaction 
•	Payment delays strongly correlate with churn behavior 
Visualizations Used
•	Churn distribution plots 
•	Correlation heatmaps 
•	Boxplots 
•	Feature importance graphs 
•	Confusion matrix 
________________________________________
Handling Class Imbalance using SMOTE
The dataset contained class imbalance, which can negatively affect machine learning performance.
To solve this issue, SMOTE (Synthetic Minority Oversampling Technique) was applied to the training dataset.
SMOTE generates synthetic samples of the minority class to create a balanced dataset and improve model learning.
Benefits of SMOTE:
•	Improves recall and F1-score 
•	Reduces model bias toward majority class 
•	Enhances churn detection capability 
________________________________________
Machine Learning Models Used
K-Nearest Neighbors (KNN)
KNN predicts churn based on the nearest neighboring data points using distance calculations.
Random Forest
Random Forest combines multiple decision trees to improve prediction accuracy and reduce overfitting.
XGBoost
XGBoost is an advanced boosting algorithm that improves model performance using gradient boosting techniques.
________________________________________
Model Evaluation
The models were evaluated using the following metrics:
•	Accuracy 
•	Precision 
•	Recall 
•	F1-score 
•	ROC-AUC Score 
•	Confusion Matrix 
Final Model Selection
The Random Forest model was finalized because it achieved the best balance between accuracy, precision, recall, and ROC-AUC score.
### Final Random Forest Performance

| Metric    | Score |
|------------|--------|
| Accuracy   | 84%    |
| Precision  | 82%    |
| Recall     | 78%    |
| F1-score   | 80%    |
| ROC-AUC    | 0.87   |
________________________________________
Tools and Libraries Used
Programming Language
•	Python 
Libraries
•	Pandas 
•	NumPy 
•	Matplotlib 
•	Seaborn 
•	Scikit-learn 
•	Imbalanced-learn 
Development Environment
•	Jupyter Notebook 
•	VS Code 
________________________________________
Key Business Insights
High Churn Risk Customers
Customers with:
•	low usage frequency 
•	short subscription tenure 
•	frequent support calls 
•	payment delays 
were identified as high-risk customers.
________________________________________
Business Recommendations
1. Improve Customer Engagement
Provide personalized recommendations and offers to low-usage customers.
2. Enhance Customer Support
Improve issue resolution speed to reduce dissatisfaction.
3. Offer Retention Campaigns
Provide discounts or loyalty rewards for at-risk customers.
4. Encourage Long-Term Contracts
Promote annual subscription plans to improve customer retention.
________________________________________
Business Value of the Project
This solution helps businesses:
•	Predict customer churn proactively 
•	Improve retention strategies 
•	Reduce revenue loss 
•	Increase customer lifetime value 
•	Support data-driven business decisions 
________________________________________
Conclusion
This project demonstrates how machine learning can be used to predict customer churn and support customer retention strategies.
By combining:
•	Data preprocessing 
•	EDA 
•	SMOTE 
•	Feature scaling 
•	Machine learning models 
the system effectively identifies customers likely to churn and provides actionable business insights.
________________________________________
Future Improvements
Future enhancements may include:
•	Hyperparameter tuning 
•	Deep Learning models 
•	Real-time churn prediction dashboards 
•	Model deployment using Streamlit or Flask 
•	Integration with business CRM systems 
