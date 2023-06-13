# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:

Import panda module as pd
### Step 2:

Import linear model from sklearn
### Step 3:

Read the file cars.csv
### Step 4:

Assign the values for x and y as required
### Step 5:

Create the linearRegression model and predict the output
## Program:
```
'''
Programmed by: ShashinPrasad S
Register number: 212222230144
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:

![py3](https://github.com/shashinprasad/Multivariate-Linear-Regression/assets/129143499/699c39cb-a09c-4677-9978-3e3585498cc1)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
