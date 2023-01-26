# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1


### Step2


### Step3


### Step4


### Step5


## Program:
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