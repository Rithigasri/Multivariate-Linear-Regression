# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas module.

### Step2
Import linear_model from sklearn and read the csv file.

### Step3
Use built-in function LinearRegression().

### Step4
Also use regr.coef_ and regr.intercept_ to find coefficient and intercept values respectively.

### Step5
Give the user input using predict().

### Step6
Execute the program.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("The predicted CO2 for the corresponding and weight and volume",predictedCO2)
```
## Output:

![OUTPUT](./OUTPUT.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.