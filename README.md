# Telecom-churn
## Introduction
For Telecom companies it is key to attract new customers and at the same time avoid contract terminations (=churn) to grow their revenue generating base. Looking at churn, different reasons trigger customers to terminate their contracts, for example better price offers, more interesting packages, bad service experiences or change of customers’ personal situations.

Churn analytics provides valuable capabilities to predict customer churn and also define the underlying reasons that drive it. The churn metric is mostly shown as the percentage of customers that cancel a product or service within a given period (mostly months). 
Telecoms apply machine learning models to predict churn on an individual customer basis and take counter measures such as discounts, special offers or other gratifications to keep their customers. A customer churn analysis is a typical classification problem within the domain of supervised learning.\
## Steps for creating a machine learning model.
• Step 1: Problem Definition

• Step 2: Read Data 

• Step 3: Exploratory Data Analysis (EDA)

• Step 4: Data Cleaning

• Step 5: Model Building

• Step 6: Model Evaluation Metrics Definition

• Step 7: Model Selection

* Step 8: Testing

## Meaning of Features
By inspecting the columns and their unique values, a general understanding about the features can be build. The features can also be clustered into different categories: Classification labels

* Churn — Whether the customer churned or not (Yes or No)
### Customer services booked
* PhoneService — Whether the customer has a phone service (Yes, No)
* MultipleLines — Whether the customer has multiple lines (Yes, No, No phone service)
* InternetService — Customer’s internet service provider (DSL, Fiber optic, No)
* OnlineSecurity — Whether the customer has online security (Yes, No, No internet service)
* OnlineBackup — Whether the customer has online backup (Yes, No, No internet service)
* DeviceProtection — Whether the customer has device protection (Yes, No, No internet service)
* TechSupport — Whether the customer has tech support (Yes, No, No internet service)
* StreamingTV — Whether the customer has streaming TV (Yes, No, No internet service)
* StreamingMovies — Whether the customer has streaming movies (Yes, No, No internet service)
* Customer account information
* Tenure — Number of months the customer has stayed with the company
* Contract — The contract term of the customer (Month-to-month, One year, Two year)
* PaperlessBilling — Whether the customer has paperless billing (Yes, No)
* PaymentMethod — The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
* MonthlyCharges — The amount charged to the customer monthly
* TotalCharges — The total amount charged to the customer
* Customers demographic info
* customerID — Customer ID
* Gender — Whether the customer is a male or a female
* SeniorCitizen — Whether the customer is a senior citizen or not (1, 0)
* Partner — Whether the customer has a partner or not (Yes, No)
* Dependents — Whether the customer has dependents or not (Yes, No)

## Step 1: Problem Definition
* Based on the introduction the key challenge is to predict if an individual customer will churn or not. To accomplish that, machine learning models are trained based on 70% of the sample data. The remaining 30% are used to apply the trained models and assess their predictive power with regards to “churn / not churn”.

## Step 2: Data Collection
The data set for this classification problem is taken from Kaggle.

https://www.kaggle.com/blastchar/telco-customer-churn

## Step 3: Exploratory Data Analysis
After data collection, several steps are carried out to explore the data. Goal of this step is to get an understanding of the data structure, conduct initial pre-processing, clean the data, identify patterns and inconsistencies in the data.

## Step 4: Data Cleaning
Based on the data types and the values, following actions are defined to pre-process/engineer the features for machine readability and further analysis:

* Total Charges should be numeric.
* Creating Dummies
* Converting target variable “Churn” into binary. (Yes=1 and No=0)
* Removing the "customer ID" column.

## Step 5: Model Building
* Train/Test Split
For conduction of model training and testing steps, the data set is split into 70% training data and 30% test data. The “Churn” column is defined as the class (the “y”), the remaining columns as the features (the “X”).

## Data balancing
* The data is imbalanced, so we have to balance the data for better model prediction, accuracy etc.

* Training, Prediction and Assessment.

## Step 6: Model Evaluation Metrics
For performance assessment of the chosen models, various metrics are used:

* Confusion matrix: Shows a grid of true and false predictions compared to the actual values
* Accuracy score: Shows the overall accuracy of the model for training set and test set.
* Recall: Recall is the number of true positives divided by the number of true positives plus the number of false negatives.
* Precision: Precision is defined as the number of true positives divided by the number of true positives plus the number of false positives.
* F1 Score: Builds the harmonic mean of precision and recall and thereby measures the compromise between both.

## Step 7: Model Selection
* Based on the confusion matrix, recall, precision and accuracy score, we will select the model which perform better.
