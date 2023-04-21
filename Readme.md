# Description of the project


Customers began to leave Beta-Bank. Every month. A little, but noticeable. Banking marketers figured it was cheaper to keep current customers than to attract new ones.

It is necessary to predict whether the client will leave the bank in the near future or not. You are provided with historical data on customer behavior and termination of agreements with the bank.

Build a model with an extremely large _F1_-measure. To pass the project successfully, you need to bring the metric to 0.59. Check the _F1_-measure on the test set yourself.

Additionally measure _AUC-ROC_, compare its value with _F1_-measure.

## Signs and conditions
-   _RowNumber --_ row index in data
- _CustomerId_ — unique customer ID
- _Surname —_ surname
- _CreditScore —_ credit score
- _Geography —_ country of residence
- _Gender —_ gender
- _Age —_ age
- _Tenure —_ how many years a person has been a bank client
- _Balance —_ account balance
- _NumOfProducts —_ the number of bank products used by the client
- _HasCrCard —_ the presence of a credit card
- _IsActiveMember —_ client activity
- EstimatedSalary —_ estimated salary
## Target feature
-   _Exited_ — факт ухода клиента 

# Conclusions based on the results of the analysis

Considering data with imbalance + translated categorical + standardized data and without imbalance by three models, we can conclude that the best model is Random Forest. With the best value max_depth=12,n_estimators=24, we have F1 = 0.601 samples. The Logistic Regression model performed the worst.

The test model showed F1 = 0.639, which is higher than the data obtained on the best previous sample (0.6601). And above the metric F1 = 0.59 specified in the condition.

The tested model highlighted the share of the correct forecast for the outflow of customers = 67% of the options recognized as positive = 61%.

This means that the bank as a whole, and the marketing department, in particular, need to reconsider the principles of organizing work, collect feedback on the reasons for terminating contracts. Draw conclusions.


