# Customer Churn Prediction
Maintaining customer retention is crucial as it fosters brand loyalty, reducing the need for continuous marketing efforts and generating a consistent revenue stream. Satisfied and loyal customers not only contribute to sustained profitability but also serve as advocates who can positively influence new customer acquisition through word-of-mouth recommendations.

# Background
In this project, we are given dataset of customer profile. We are asked to analyze behaviour of churned customer and build machine learning model to predict whether a customer will churn or not based on the data available.

# Data
The dataset can be accessed through [Kaggle](https://www.kaggle.com/datasets/muhammadshahidazeem/customer-churn-dataset/data?select=customer_churn_dataset-training-master.csv). The dataset contains 12 features:  CustomerID, Age, Gender, Tenure, Usage Frequency, Support Calls, Payment Delay, Subscription Type, Contract Length, Total Spend, Last Interaction and Churn. This dataset have 505.256 rows of data, separated into two file (training data with 440.882 rows of data and testing data with 64.374 rows of data).

# Process
The notebook is structured this way:
1. **Business Understanding**: Explain the importance of customer churn prediction
2. **Data Understanding**: Provide an explanation of the dataset used, data sources, and features.
3. **Data Pre-Processing**: Perform initial data inspection as an overview of the data to be used, perform initial data cleaning, divide the data into train-test data and train-validation-test data for modeling purposes, check for missing values and duplicate data.
4. **Exploratory Data Analysis**: Perform visualization and analysis of the dataset.
5. **Feature Analysis**: Looking at the correlation between features
6. **Modeling**: Build several Machine Learning baseline models (Logistic Regression, Random Forest, and XGBoost) for customer churn prediction & measure their performance.
7. **Modeling with Oversampling**: Building Machine Learning models using oversampling method (SMOTE).
8. **Key Insight & Recommendation**: Key insights and results of Machine Learning modeling for customer churn prediction and recommendations for actions that can be taken to reduce and prevent customer churn.

# Key Findings
1. A feature which is the strongest predictor of customer churn: Support Calls. This can refer to bad customer service (customer with more Support Calls tend to churn) or bad service. The company have to investigate to understand why there are many customers with very high Support Calls and address the issue immediately.

Boxplot of Customers' Support Calls, categorized by Churn

![image](https://github.com/faisalghifariz/customer-churn-prediction/assets/90921520/373d8398-1fbe-4b8f-bc06-c6e796f9782e)

The distribution plot of Customers' Support Calls. It can be seen that there are many churned customers with very high Support Calls.

![image](https://github.com/faisalghifariz/customer-churn-prediction/assets/90921520/ec5736a2-cec6-48d5-b2eb-3644251d4a72)

2. 3 Machine Learning methods used (Logistic Regression, Random Forest, and XGBoost) show great performance on predicting churned customer.
   - Logistic Regression have 98% recall (standard) and 97% recall (oversampling using SMOTE)
   - Random Forest have 100% recall (standard) and 100% recall (oversampling using SMOTE)
   - Logistic Regression have 100% recall (standard) and 100% recall (oversampling using SMOTE)
   It means all three models predict over 95 churned customer out of 100 predicted churned customer. The company can use one of the models to predict churned customers.


Interested to see presentation version of this project? You can view the presentation version [here](https://www.linkedin.com/feed/update/urn:li:activity:7140013902850842624/) in my lLinkedin!
