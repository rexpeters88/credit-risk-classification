# credit-risk-classification

Project Report 

Overview of the Analysis:
This analysis evaluates the performance of a logistic regression model in predicting credit risk. In particular, the model classified loans as either high-risk or low-risk, based on features included in the primary dataset. 


Purpose of the analysis:
The dataset contains financial information about loans and borrowers, and the goal of the analysis is to predict whether a loan is high-risk or low-risk. The target variable for prediction is loan_status, which indicates the loan's risk category.

Dataset Columns:
1. loan_size: The size of the loan issued (numerical).
2. interest_rate: The interest rate charged on the loan (numerical).
3. borrower_income: The annual income of the borrower (numerical).
4. debt_to_income: The borrower's debt-to-income ratio, calculated as total debt divided by income (numerical).
5. num_of_accounts: The number of financial accounts (e.g., credit cards, loans) the borrower has (numerical).
6. derogatory_marks: The number of negative marks (e.g., late payments, defaults) on the borrower’s credit history (numerical).
7. total_debt: The total outstanding debt of the borrower (numerical).
8. loan_status: The target variable indicating the loan’s risk level:
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
The logistic regression model performed exceptionally well, achieving an overall accuracy of 99%. It showed perfect precision (1.00) and high recall (0.99) for low-risk loans (Class 0), while maintaining strong performance for high-risk loans (Class 1) with precision of 0.84 and recall of 0.94. This indicates that while the model is highly reliable for predicting low-risk loans, there is still room for improvement in terms of identifying high-risk loans. Furthermore, given that identifying high-risk loans (Class 1) is more critical, additional adjustments (e.g., oversampling, adjusting class weights) could further improve performance for this class. 


