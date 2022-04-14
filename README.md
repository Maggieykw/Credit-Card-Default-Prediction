# Credit-Card-Default-Prediction

## Task
We are interested in predicting defaults in the next month, which is October of 2005. Apply three models for this task and compare them: 
1. Classification trees with boosting
2. Logistic regression
3. Deep learning (feedforward neural network)

The dataset has 30,000 records in total and it is randomly splitted into the training set (20,000) and the test set (10,000) with the ratio of 33:50.

Deep learning model and the logistic regression model is performed using Python
Classification Trees with Boosting is performed using R

At the end, we will compare the overall error rate and AUC of three models on the training and test sets;
And dertermine the variables are important for predicting defaults (in classification trees)

Remark: Sex, education and marriage are three categorical variables. One way to deal with such variables as inputs to a neural network is using one-hot vectors. The Jupyter notebook “NN-Data” provides you with the Python code to process the data.

For the modelling and model performance, please refer to the file 'Predictive Model.ipynb'

## Dataset

This dataset (see the csv file 'UCI_Credit_Card.csv') contains information on default payments, demographic fac- tors, credit data, history of payment, and bill statements of credit card clients in Taiwan from April 2005 to September 2005.

There are 25 variables:
• ID: ID of each client
• LIMIT BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit)
• SEX: Gender (1=male, 2=female)
• EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown,
6=unknown)
• MARRIAGE: Marital status (1=married, 2=single, 3=others)
• AGE: Age in years
• PAY 0: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, . . . 8=payment delay for eight months, 9=pay- ment delay for nine months and above; you also see -2 in the dataset and its meaning is not explained by the data provider but it could refer to prepayment)
1
• PAY 2: Repayment status in August, 2005 (scale same as above) • PAY 3: Repayment status in July, 2005 (scale same as above)
• PAY 4: Repayment status in June, 2005 (scale same as above)
• PAY 5: Repayment status in May, 2005 (scale same as above)
• PAY 6: Repayment status in April, 2005 (scale same as above)
• BILL AMT1: Amount of bill statement in September, 2005 (NT dollar)
• BILL AMT2: Amount of bill statement in August, 2005 (NT dollar)
• BILL AMT3: Amount of bill statement in July, 2005 (NT dollar)
• BILL AMT4: Amount of bill statement in June, 2005 (NT dollar)
• BILL AMT5: Amount of bill statement in May, 2005 (NT dollar)
• BILL AMT6: Amount of bill statement in April, 2005 (NT dollar)
• PAY AMT1: Amount of previous payment in September, 2005 (NT dollar) • PAY AMT2: Amount of previous payment in August, 2005 (NT dollar)
• PAY AMT3: Amount of previous payment in July, 2005 (NT dollar)
• PAY AMT4: Amount of previous payment in June, 2005 (NT dollar)
• PAY AMT5: Amount of previous payment in May, 2005 (NT dollar)
• PAY AMT6: Amount of previous payment in April, 2005 (NT dollar)
• default.payment.next.month: Default payment (1=yes, 0=no)
