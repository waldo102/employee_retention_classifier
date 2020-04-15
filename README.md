# employee_retention_classifier
Goal: Classify which employees are most likely to leave a company by using data from Human Resources


Data:
  * hr_data - contains 9 variables and 14k observations.
  * employee_satisfaction_evaluation.xlsx - contains 3 variable and 14k observations

Files:
  * Human_Resources_Retention.ipynb - performs data cleaning, data preparation, data analysis, and also model specifications
  
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

The best performing model was the Random Forest Classifier with a classification accuracy of 99% and an F1-Score of 0.98.
The Neural Network registered an accuracy of 95% and an F1-Score of 0.91. Finally, the Logistic Regression performed the worst
with an accuracy of 79% and an F1-Score of 0.45.

Conclusions:

Overall, we reached a very good level of classification accuracy with the Random Forest Classifier, that was significantly better
than the Logistic Regression model. Typically, the choice between models comes down to how much more precision we gain from
the added complexity of the model. Despite being more complex, the specified Neural Network model does not perform better
than the random forest model. It maybe because of the nature of the data; Neural Networks tend to perform better with large amounts
of data (greater than 1 million observations) and when nonlinear relationships are more prevalent. Ultimately, the decision to not
continue searching for a deeper Neural Network that would give a better degree of accuracy than the Random Forest was made because 
of the very high (99%) accuracy of the random forest model. The added complexity would not be justified given how small the room
for improvement is. Thus, the Random Forest is the best model for this data and task.

In addition, according to the data, the most important variables that determine the retention of an employee are

* the level of satisfaction of the employee (measured through surveys), 
* the amount of time the employee has been working for the company, and 
* the number of projects the employee has been a part of

Note: plotly animations will not load on github. However, running the Jupyter Notebook locally will render the plots correctly. 
