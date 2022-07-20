# Risk based prediction of interest for loan
 
## Business objective
A company is in the financial lending business and provides loans to retail customers. It currently uses a process of first collecting certain customer information (attributes), analyzing it manually to decide whether the customer is eligible for a loan or not, and if eligible, telling the customer at what rate of interest rates it can avail the requested loan. Going forward the company wants to employ an automated process which is based upon a Machine Learning model. Not only is this model expected to make the decisioning process faster, but also keep it free from human error and biases.

## Approach
* Data collection
* Data wrangling
* Exploratory Data Analysis
* Feature engineering
* Feature scaling
* Choose the model
* Model Evaluation
* Parameter tuning
* Prediction

## Analysis/ Modeling Methodology

### Data Preparation & EDA
* Sub-setting is done by removing Loan_ID.
* All the missing values have been replaced with corresponding mean or mode.
* Extensive bi-variate analysis conducted on all meaningful variables.

### Variable Creation and  Selection
* 20+ new variables created as a part of feature engineering.
* Used label encoding to create dummy variables.
* Used mapping techniques to map the object variables to numerical variables.

### Model Development
* Decision tree classifier chosen as the preferred modeling technique since the target variable  is  multiclass and data is complex.
* Developed 5+ candidate models.
* Highest Model accuracy observed of 74%.

### Model performance testing
* Conducted k-cross validation for k=5,10,15.
* Model performance also assessed on a hold-out sample of size 20% of the original dataset.
* Performed all the required metrics precision ,recall, confusion matrix ,roc_auc curve.

## Extended Data Dictionary
![image](https://user-images.githubusercontent.com/93145713/169710826-97780919-beb8-4105-9bd8-3df4351c431b.png)

### Data distribution with respect to interest rates
                                       Interest rate 1
![image](https://user-images.githubusercontent.com/93145713/169710942-ea356836-a2f6-4773-9650-13cf4ac56d93.png)

                                       Interest rate 2
![image](https://user-images.githubusercontent.com/93145713/169710965-be364bf6-ccc7-4725-b135-97d03e5d9fba.png)

                                       Interest rate 3
![image](https://user-images.githubusercontent.com/93145713/169710971-f9e12f63-9d95-4f0a-beee-f64d6a992656.png)

![image](https://user-images.githubusercontent.com/93145713/169711129-0ce23c40-a5d7-4a50-a8cd-5cae8e3b49b2.png)

![image](https://user-images.githubusercontent.com/93145713/169711151-36fc5705-b1b0-49e2-9e6d-5d454acb4109.png)

![image](https://user-images.githubusercontent.com/93145713/169711180-a7d5dcd4-42ae-4743-b18a-8d38e2565213.png)

Corelation matrix

![image](https://user-images.githubusercontent.com/93145713/169711287-a9b01ed0-ee7d-4d83-8e75-b02e25ce45a1.png)


## Model Building
* Developed a decision tree classifier model on the data set provided
* Split the data into 80% and 20%. 80% of records for train the model and remaining records are for testing.
* Trained the model with data.
### Model evaluation
                            Classification Report
![image](https://user-images.githubusercontent.com/93145713/169711588-b2c06d11-5832-436e-8a22-fcea6bc46a41.png)

![image](https://user-images.githubusercontent.com/93145713/169711610-21a626e3-005c-41de-a3c1-2cb12905f8f1.png)

![image](https://user-images.githubusercontent.com/93145713/169711621-24646cc2-c1af-43f5-9300-389aa6b77040.png)

Cross validation score
For the further validation, Cross Validation technique is used with k-Fold values 10,15, and 20
The average score that is obtained  around 42%.

The model performance is little poor. Because data is fully baised
