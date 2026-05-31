# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Load the required Python libraries (pandas, sklearn) and read the dataset (car.csv) into a DataFrame.

### Step2
<br>Choose independent variables (Weight, Volume) as features and dependent variable (CO2) as the target.

### Step3
<br>Create a LinearRegression() object and fit it with the selected features and target to compute coefficients and intercept.

### Step4
<br>Print the regression coefficients and intercept to understand the relationship between features and target.

### Step5
<br>Use the trained model to predict CO2 emissions for new input values (e.g., Weight=3300, Volume=1300) and display the result.

## Program:
```
Implementation of Multivariate Linear Regression
Developed by: THAMIZHMANI M
Register Number: 212225040468

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:

### Insert your output
<img width="799" height="85" alt="Screenshot 2026-05-29 191616" src="https://github.com/user-attachments/assets/c647daf8-3007-480e-8007-63fbb781d3e6" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
