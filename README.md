# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
### Step 1:
Import the libraray pandas using inport command.

### Step 2:
From sklearn import another library linear_model.

### Step 3:
Read the csv file which is uploaded.

### Step 4:
Fit the x and y in csv file which we assigned.

### Step 5:
Print Coefficient and intercept of the regression.

### Step 6:
Run the program and predict the output

## Program:
```
Program to implement multivariate Linear Regression to fit a straight line using least squares.
Developed by: Santhosh U
RegisterNumber: 22009224
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars.csv")
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
![MultivariateRegression](https://user-images.githubusercontent.com/119477975/214834269-3bbc4bff-6b3c-42b0-8b7a-fc424889123e.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
