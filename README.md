# credit-risk-classification

Project Report 

Overview of the Analysis:
valuate the performace of a logistic regression model that is designed to predict credit risk.


Purpose of the analysis:
The goal of the anlysis is to analyze how well the logistic regression model was abke to classify loans as high-risk or low-risk.

Dataset Columns:
1. loan_size
2. interest_rate
3. borrower_income
4. debt_to_income
5. num_of_accounts
6. derogatory_marks
7. total_debt
8. loan_status (target variable):
      a. 0: Low-risk loan
      b. 1: High-risk loan



Machine Learning Process: 
The first faze of this process was centered around data preparation and involved feature selection/target separation. It also included splitting the data into training and testing sets using train_test_split, in order to later evaluate the models performance on unseen data. While we considered scaling the data, we ultimately decided against it for the particular requirement of this assignment. The second step involved model selection and training. The LogisticRegression algorithm was selected as it is well-suited for binary classification problems like predicting loan risk. We used the trained logistic regression model to predict loan_status for the testing dataset (X_test), resulting in a set of predicted labels (y_pred). Its performance was then evaluated using a confusion matrix, classification report, and accuracy score


Results:
Model Performance Metrics
Logistic Regression:
Accuracy: 99%
Precision:
Class 0 (Low-Risk): 1.00
Class 1 (High-Risk): 0.84
Recall:
Class 0 (Low-Risk): 0.99
Class 1 (High-Risk): 0.94


Summary:
The model achieved an overall accuracy of 99%, indicating it performed extremely well. However, its precision was much higher when predicting low-risk loans relative to high-risk loans. This indicates that while the model is a good start, further improvements are important in order to increase its identification of high-risk loans, which pose greater threats to loan providers. 


