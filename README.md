# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
 Import Pandas library and linear_model from sklearn using import statement.

### Step2
Read the given csv file using read_csv() method.

### Step3
Create two arrays, independent array x with two classes and dependent array y with one class. Find the regression of x and y using linear_model.LinearRegression() method and fit x and y usind .fit() method.

### Step4
Find the coefficients using .coef_ and intercept using .intercept_

### Step5
Predict the liner regression using regr.predict() method and display the result.

## Program:
```
developed by: YAZHINI R R 
reg no: 212224100063
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("C:\\Users\\admin\\Downloads\\carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```
## Output:
![ex 10](https://github.com/user-attachments/assets/7f423d12-cdba-4730-b19a-d06433586b6f)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
