# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>import pandas as pd.

### Step2
<br>Read ths csv file.

### Step3
<br>Get the value of X and Y variables.

### Step4
<br>Create the linear regression model and fit.

### Step5
<br>Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
'''
DEVELOPED BY:KRISHNARAJ D
REGISTER NO:22005130
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car..csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predict CO@ for the corresponding weight and volume",predictedCO2)
```
## Output:
![out](/1.png)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
