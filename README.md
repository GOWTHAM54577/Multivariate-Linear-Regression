# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
###Step 1:
Import the numpy module to use the built-in functions for calculation

###Step 2:
Prepare the lists from each linear equations and assign in np.array()

###Step 3:
Using the np.linalg.solve(), we can find the solutions.

###Step 4:
End the program


## Program:
```
#Developed by: GOWTHAM N
#Reg no:23001663
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:
![OUTPUT](https://github.com/GOWTHAM54577/Multivariate-Linear-Regression/assets/144589420/bbc43158-8cd7-4e4a-b0ae-fef08cf00bb5)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
