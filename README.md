# Customer-Churn-Prediction
A Machine Learning based application to predict customer churn for a telecommunications services company.

# Objective
Customer churn occurs when customers stop doing business with a company.As the cost of retaining an existing customer is far less than acquiring a new one, maintaining a healthy customer base is important for the success of any business.As customers have multiple options in the telecom industry, the churn rate is particularly high in this industry.Individualized customer retention is difficult because businesses usually have a lot of customers and cannot afford to spend much time on one. The costs would be too high and would outweigh the extra revenue.But if a company could predict in advance which customers are at risk of leaving, they could focus customer retention efforts by directing them solely toward such "high risk" customers.

# Dataset
The dataset used was taken from kaggle.
Dataset link: https://www.kaggle.com/blastchar/telco-customer-churn

The main objective of my project was to build a predictive model to generate a prioritized list of customers most vulnerable to churn.

# Method
Much of data cleaning was not required as the provided data was mostly complete and properly formatted. However, features like “Total Charges” were initially in String format and few entries contained empty strings, which needed to be taken care of. There was some degree of multi-collinearity between features like “Monthly Charges & Total Charges” and “Streaming TV & Streaming Movies”, which could be taken advantage of to reduce data complexity. Some features like “Customer ID” were dropped as they had no significance as far as prediction is concerned. Dummy variables were used to encode string type features to Integer values. One Hot Encoding could also be used instead.
The following Machine Learning models were used:
  1.	Logistic Regression
  2.	KNN
  3.	Support Vector Machines
  4.	Naive Bayes classifier
  5.	Decision Tree
  6.	Random Forest
  7.	Linear Discriminant Analysis
  8.	Ada Boost Classifier
  9.	Gradient Boosting Classifier
  
Out of the above-mentioned models Random Forest & Logical Regression gave us the best accuracy and cross validated score. Further Hyper-Parameter Tuning was applied on The Random Forest Classifier and the best fitting estimators were found out, which are described and shown in the uploaded Jupiter notebook. Random Forest model gave us the best score because the data we were dealing with was not balanced data, for such cases Tree based algorithms like Random Forest & Decision Tree are most suited.

With help from the visual analysis of the data, the relationship between each input variable and target variable was observed using statistics, the variables with strongest relations were selected, i.e., Filter feature selection method. The visual and statistical analysis for the same is given in the uploaded jupyter notebook.

# Performance of the model
Random Forest Classifier was chosen as the final model for prediction, which after applying the estimator from parameter tuning, gave us a score of 87.88%
The cross validated score for the same was 82.24%. Other accuracy and performance metrics like Confusion matrix and AU-ROC Curve (for classification models) is given in the uploaded jupyter notebook.

# Here's what we learnt
The key factors predicting a customer’s churn are Total Charges, Monthly Charges & Tenure. The greater total charges and tenure are, the less is the probability to churn. Users with a month to month contract are more likely to churn than users with long term contracts.
These factors clearly make sense as apart from services, cost is the main factor guiding a customer’s decision. Tenure is another important factor as a customer will only opt for a longer tenure if he/she is satisfied with the company’s services and price.

Customers should be encouraged to opt for long term contract with reasonable long-term price offers. Further service benefits must be given to long term customers. Customers should be made aware of various optional benefits with the service such as Online Security, Online Backup, Streaming TV etc. and such add on services must be advertised accordingly. Some of these add on offers should be made free of cost with the service.
Referral and family plan schemes must be introduced to encourage Chain marketing.
   






    
           
           

