
## EXP-10: Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Start the program

### Step2
<br>Write a program to perform multivariate regression in anaconda navigator.

### Step3
<br>Run the program

### Step4
<br>Print the output.

### Step5
<br>End the program.

## Program:
```
DEVELOPED BY: Malligesh
REGISTER NUMBER: 212223230119
```
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("caremission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:



<br>![image](https://github.com/user-attachments/assets/202fce0f-8dfb-4461-9faf-79fb6994adbf)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
