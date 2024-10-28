# Practical-Application-Assignment-17.1-Comparing-Classifiers

Link to the assignment: https://github.com/sraashi/Practical-Application-Assignment-17.1-Comparing-Classifiers/blob/main/Practical%20Assignment%2017.1-checkpoint.ipynb

Here the task is to use the CRISP-DM strategy on a banking dataset, applying various models to predict which customer will subscribe to a term deposit given various parameters. 

Business understanding: The task here is to predict a customer subscribing to a term deposit given various parameters including client information, marketing campaign communication and responses from previous campaigns so as to tailor the outreach and target the right customers.

Data understanding: The various features that are collected here include client information such as age, marital status, occupation, education, balance, loan, if the client has defaulted in credit, along with their responses to previous marketing campaigns, when they were last contacted, how long since it's been, etc. The target variable is whether the customer subscribed to a term deposit or not. 

Summary of data: 
45211 rows of data, with no null values. 
Numerical Features: ‘age’, ‘balance’, ‘day’, ‘duration’, ‘campaign’, ‘pdays’, ‘previous’.
Categorical Features: ‘job’, ‘marital’, ‘education’, ‘default’, ‘housing’, ‘loan’, ‘contact’, ‘month’, ‘poutcome’, ‘y’.
These categorical features would need to be one hot encoded. 

Data preparation: At the data preparation stage, I primarily employed three steps: One hot encoding to convert the categorical values to features that could be represented with numerical values, standardization to scale the data around zero and outlier management to ensure extreme values do not skew predictions. For this I used box plots to evaluate what range of values to use for each column. 

Data modeling: kNN, logistic regression, decision trees and svm were models that were used to evaluate the data. 

Data analysis: From the accuracy scores, logistic regression and support vector machines have the highest accuracy scores. SVM has a slight edge over the others in predicting those who would subscribe. Depending on the goals of the bank, the input features and the models can be further refined to predict the clients that will subscribe to term deposits. 
