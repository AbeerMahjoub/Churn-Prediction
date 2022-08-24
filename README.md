# Churn Prediction
![Churn](https://github.com/AbeerMahjoub/Churn-Prediction/blob/main/Customer-churn-rate.jpg)

# Overview:
  
  **In business it is usually easier to keep customers than acquiring new customers, so it's very important to be able to predict 
  customers who are likely to cancel the service, and deal with them.**
  
 # Data:

  ## Data can be splitted into three sets:
   ### Customer Demographics:
   - Gender.
   - SeniorCitizen.     
   - Partner.
   - Dependents.
   ### Service Related:
   - tenure.
   - PhoneService
   - MultipleLines.
   - InternetService
   - OnlineSecurity
   - OnlineBackup
   - DeviceProtection
   - TechSupport
   - StreamingTV
   - StreamingMovies
   ### Contranct and Billing:
   - Contract
   - PaperlessBilling
   - PaymentMethod
   - MonthlyCharges
   - TotalCharges
   ### Target:
   - Churn
   
   **Data resource: [Kaggle](https://www.kaggle.com/code/bandiatindra/telecom-churn-prediction)**

# Insights:
After careful analysis we could extracts some patterns and insights that can help us identify customers who are more likely to leave the service.
We've found that:
- Senior citizens, single customers and customers with no dependents are more likely to churn.
- Customers who are on month-to-month contracts having a high churn rate compared to one or two years contracts.
- Customers who don't subscribe for many services have a high churn rate.

# Modeling and Evaluating:
We will evaluate the model based on recall metric, as we want the model to be able to predict as much churners as possible.
- Logistic Regression Model - 64% recall
- Random Forest Model - 69% recall
- Support Vector Machine - 61% recall
- Adabooost Model - 63% recall
- XGB-Classifier - 65 % recall

We can see that the random forest classifier was able to outperform other model, by being able to predict 69% of churners.

# Improvements:
Improving the model can be through:
- Hyperparameter tuning 
- More Feature engineering
