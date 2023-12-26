# LP-Two-Project - CUSTOMER CHURN - An Analysis For Vodafone
# INTRODUCTION
Customer retention is an integral aspect of every business, and this strategy focuses on maintaining existing customers. Today businesses depend on machine learning to predict if a customer will be retained or lost, this enables business owners to plan as to how to keep their existing customers and lure new customers.
In other to predict if customers will churn or not, a supervised learning approach known as Classification comes to play as it enables stakeholders to predict the future of the business ahead of time.

# OBJECTIVES
The aim of the project is to develop a supervised machine learning model that analyse customer attrition in Vodafone.
The project seeks to identify probable customer churn, offer insightful information about customer behaviour, and create a proactive customer retention initiative.
The project's output will help Vodafone deal with customer turnover in a more knowledgeable and proactive manner.


# HYPOTHESIS
With the initiative to find out if customer churn has a relationship with the contract type, these hypothesis statements were formulated.
Null Hypothesis: There is no significant relationship between customers churn and the type of contract.
Alternative Hypothesis:  There is a significant relationship between customers churn and the type of contract.
After the hypothesis testing was done, we failed to reject the Null Hypothesis since the P-value is more than 0.05. 

# BUSINESS QUESTIONS
Below are the questions addressed based on the dataset:
1.What is the overall count of customers who have discontinues their services with the company?

2.Which contract type exhibits a higher number of customers who have left company?

3.How does the rate of customer churn change in relation to the duration of their subscription?

4. Is there a correlation between the total charge accrued by customers and the type of contract they have?

5.What are the preferred payment method?

# DATASET 
The datasets used for this project were sourced from 3 different sources, i.e. github repository, OneDrive file, and an SQL database. The dataset's columns and their corresponding values are listed below:
Churn: Customers who left the company

Product and services the customer signed unto: Phone Service, Multiple Lines ,  Internet Service, Online Security, Device Protection, Tech Support, Streaming TV Streaming Movies

Customer Information: Contract, Paperless Billing, Payment Method, Monthly Charges    Total Charges

Demographics: age, gender, marital status, (With dependants or without dependants)

Customer Identification:  A distinct identification number that identifies every customer.

Senior Citizen: States if the customer is old or not.

Dependants: Shows if a customer has dependants or not, i.e. parents, children.

Monthly Tenure: Shows how long the customer has been with Vodafone.

Total Charges: Monthly charges * each tenure

Multiple lines: Shows if the customers have multiple telephone lines with the company.

# DATA PROCESSING 
The collected dataset needed to be modified because it contained errors such as null values and incorrect data types in some of the fields. Simple Imputer was used to impute the null values, and the data types for columns with incorrect data types were corrected.
The categorical columns were changed to numeric columns, these changes were applied to the pipeline to ensure that in future instances the same processing is affected.


# BUILDING THE MODEL AND EVALUATION
Since the aim of the project is to build a sturdy machine learning model, to achieve this we trained four models namely: Support Vector, Decision Tree, Random Forest, and Logistic Regression. 
Out of the three, two datasets were concatenated, separated into features and target variables, and then split into train and evaluation sets, with 80% going toward training and the remaining 20% going toward evaluation.
To address the unequalness of the datasets, random sampler was used to balance the dataset. To make the model work better feature selection was used to select the best feature model and hyperparameter tuning was implemented on the best performing model. To select the best performing model, we used the F1 score and the AUC-ROC curve.

# FINDINGS AND INSIGHT 
After the feature selection and hyperparameter tuning was done, the model with the best performing ability was the Logistic Regression model with an AUC-ROC score of 0.85. This model was then used to perform prediction on the on the Test data, the outcome was out of 1497 customers the model predicted that customers will churn.
The management will have to concentrate on measures to put in place to retain the customers predicted to churn.








