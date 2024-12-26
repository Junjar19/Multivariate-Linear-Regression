# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas for data manipulation. Import linear_model from sklearn for linear regression.

### Step2
Read the CSV file (car.csv) containing car data into a pandas DataFrame.

### Step3
Select the input features (Volume and Weight) as x. Select the target variable (CO2 emissions) as y.

### Step4
reate a linear regression model instance using linear_model.LinearRegression().Fit the linear regression model on the input features x and target y using .fit().


### Step5
Print the model's coefficients (slope values for Volume and Weight).Print the intercept of the model.Predict CO2 emissions for a given input (e.g., Volume = 100, Weight = 929) using .predict() and display the result.


## Program:
```
Developed by:G.Mithik jain
Ref no:24001881

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:\\Users\\admin\\Downloads\\car (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)


```
## Output:

![alt text](<Screenshot 2024-12-26 205704.png>)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.