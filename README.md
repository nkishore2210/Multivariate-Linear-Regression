# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

Step1:

import pandas as pd

Step2:

Read the csv file

Step3:

Get the values of x and y variables.

Step4:

Create the linear regression model and fit.

Step5:

Predict the CO2 emission of a car where the weight is 3300kg, and the vlume is 1300cm3.

Step6:

Print the predicted output.

## Program:
```
Program to implement multivariate linear regression and predict the output.
Developed by: N.Kishore
Register number: 212222240049

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[["Weight","Volume"]]
b=df[["CO2"]]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:

![Screenshot 2023-06-10 165954](https://github.com/nkishore2210/Multivariate-Linear-Regression/assets/118707090/e4ac5ee6-e775-4a83-8d40-099c020d446b)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
