## Risk based prediction of interest for loan
 
### Business objective
A company is in the financial lending business and provides loans to retail customers. It currently uses a process of first collecting certain customer information (attributes), analyzing it manually to decide whether the customer is eligible for a loan or not, and if eligible, telling the customer at what rate of interest rates it can avail the requested loan. Going forward the company wants to employ an automated process which is based upon a Machine Learning model. Not only is this model expected to make the decisioning process faster, but also keep it free from human error and biases.

### Approach
- At first the preprocessing techniques need to performed on the data set which includes cleaning the data ,handling missing values and outliers
- The next step includes visualization of the features and drawing useful insights from the data 
- We have to perform some key analysis from the data and find out relations of independent features with target feature
- As it is multiclassification problem we chose decision tree classifier as the algorithm to develop the model

### Tasks performed
- Data collection
- Data wrangling
- Exploratory Data Analysis
- Feature engineering
- Feature scaling
- Choose the model
- Model Evaluation
- Parameter tuning
- Prediction

## Analysis/ Modeling Methodology

### Data Preparation & EDA
- Sub-setting is done by removing Loan_ID.
- All the missing values have been replaced with corresponding mean or mode.
- Extensive bi-variate analysis conducted on all meaningful variables.

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


### Model Building
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
