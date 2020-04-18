# Employee Retention Classifier
Goal: Classify which employees are most likely to leave a company by using data from Human Resources


Data: WA_Fn-UseC_-Telco-Customer-Churn.csv
  * Source: https://www.kaggle.com/blastchar/telco-customer-churn
  * contains 21 variable and 7k observations

Files:
  * customer_churn_classification.ipynb - performs data cleaning, data preparation, data analysis, and also model specifications
  
Models:
  * Logistic Regression
  * Random Forest Classifier
  * Neural Network

Performance Metrics:
  * Classification Accuracy
  * Precision
  * Recall
  * F1-Score
  
Results:

The three models performed very similarily:

 * Logistic Regression model (79% Accuracy, 0.57 F1-Score)
 * Neural Network model (79% Accuracy, 0.59 F1-Score).
 * Random Forest classifier (78% Accuracy, 0.52 F1-Score)

Conclusions:

Because the performance of the models was similar, it would be wise to employ a logistic regression model since it is a mathematically less complex model and the results are more easily interpretable. Typically, the choice between models comes down to how much more precision we gain from the added complexity of the model. Despite being more complex, the specified Neural Network model and Random Forest Classifier do not perform significantly better than the the logistic regression model. It maybe because of the nature of the data; Neural Networks tend to perform better with large amounts
of data (greater than 1 million observations) and when nonlinear relationships are more prevalent. For future steps, it maybe necessary to acquire more data to give the models more material to train on.

In addition, according to the data, the most important variables that determine customer churn are the following:

 * Type of Contract (Monthly or Yearly)
 * Type of Internet Service
 * Whether the customer has online security or not
 
This telecommunications company may want to perform more analysis on how these characteristics of a customer affect churn. Historically, internet and service providers have moved away from contracts in favor of month-to-month billing where customers are free to cancel at a time. There should be more studies performed to see if this affects churn in this particular company.

*Resources: This project was part of Rajeev D. Ratan's course, Data Science & Deep Learning for Business™ 20 Case Studies as presented in udemy.com*
