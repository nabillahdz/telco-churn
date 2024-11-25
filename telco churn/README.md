# Telco Churn Analysis

#### Introduction to Project

This project was created as part of my group assignment for the final exam. For this project we use "Analysis And Classification of Customer Churn Using Machine Learning Models" as our reference. The table below highlights the differences between our project and our reference:

|                              | Reference                                                                          | Our Project                                                                                                                                                                                      |
| ---------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Machine Learning Model       | Logistic Regression, Random Forest,<br />SVM, AdaBoost, XGBoost, Gradient Boosting | XGBoost                                                                                                                                                                                          |
| Data Balancing Techniques    | SMOTE                                                                              | SMOTE, SMOTE-ENN, and CTGAN                                                                                                                                                                     |
| Using Hyperparameter Tuning? | No                                                                                 | Yes                                                                                                                                                                                              |
| Highest Accuracy             | XGBoost with 0.829424 accuracy                                                    | XGBoost using hyperparameter tuning:<br />'colsample_bytree': 1.0, <br />'learning_rate': 0.05, <br />'max_depth': 3, <br />'n_estimators': 200, <br />'subsample': 0.8<br />accuracy: 0.828125 |

#### Dataset Variables

The dataset is sourced from Kaggle. Some of the variables used in this assignment are:

* **CustomerID** : A unique ID that identifies each customer.
* **Gender** : The customer’s gender: Male, Female
* **Senior Citizen** : Indicates if the customer is 65 or older: Yes, No
* **Partner** : Indicate if the customer has a partner: Yes, No
* **Dependents** : Indicates if the customer lives with any dependents: Yes, No. Dependents could be children, parents, grandparents, etc.
* **Tenure Months** : Indicates the total amount of months that the customer has been with the company by the end of the quarter specified above.
* **Phone Service** : Indicates if the customer subscribes to home phone service with the company: Yes, No
* **Multiple Lines** : Indicates if the customer subscribes to multiple telephone lines with the company: Yes, No
* **Internet Service** : Indicates if the customer subscribes to Internet service with the company: No, DSL, Fiber Optic, Cable.
* **Online Security** : Indicates if the customer subscribes to an additional online security service provided by the company: Yes, No
* **Online Backup** : Indicates if the customer subscribes to an additional online backup service provided by the company: Yes, No
* **Device Protection** : Indicates if the customer subscribes to an additional device protection plan for their Internet equipment provided by the company: Yes, No
* **Tech Support** : Indicates if the customer subscribes to an additional technical support plan from the company with reduced wait times: Yes, No
* **Streaming TV** : Indicates if the customer uses their Internet service to stream television programing from a third party provider: Yes, No. The company does not charge an additional fee for this service.
* **Streaming Movies** : Indicates if the customer uses their Internet service to stream movies from a third party provider: Yes, No. The company does not charge an additional fee for this service.
* **Contract** : Indicates the customer’s current contract type: Month-to-Month, One Year, Two Year.
* **Paperless Billing** : Indicates if the customer has chosen paperless billing: Yes, No
* **Payment Method** : Indicates how the customer pays their bill: Bank Withdrawal, Credit Card, Mailed Check
* **Monthly Charge** : Indicates the customer’s current total monthly charge for all their services from the company.
* **Total Charges** : Indicates the customer’s total charges, calculated to the end of the quarter specified above.
* **Churn Label** : Yes = the customer left the company this quarter. No = the customer remained with the company. Directly related to Churn Value.
