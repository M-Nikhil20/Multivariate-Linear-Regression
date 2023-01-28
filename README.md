# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas and linear model (from sklearn


### Step2
Assign the variables x and y as the Weight and volume, CO2


### Step3
Find the regression using regr = linear_model.LinearRegression()


### Step4
USe fit(x,y)


### Step5
to print output

## Program:
Developed by: M Nikhil
Register number: 22008584
```

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)

```
## Output:
![OUTPUT](/Screenshot%202023-01-26%20185851.png)

### Insert your output
![OUTPUT](/Screenshot%202023-01-26%20185931.png)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
