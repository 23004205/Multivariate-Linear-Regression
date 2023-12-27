
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4

Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm3.

### step6
Print the predicted output.

## Program:
```
##program to find the 
##developed by:singamala venkata sai kumar reddy
##register number :212223230208

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
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
![Screenshot 2023-12-27 150450](https://github.com/23004205/Multivariate-Linear-Regression/assets/138971114/01c6b672-8d03-4836-b20a-40aa87783255)

### Insert your out:
```
Coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted CO2 for the corresponding weight and volume [114.75968007]
```
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
