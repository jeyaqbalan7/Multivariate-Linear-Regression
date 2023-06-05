# EX.NO-10 Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import pandas as pd.

### Step2
<br>
Read the csv file.

### Step3
<br>
Get the value of X and Y variables.

### Step4
<br>
Create the linear regression model and fit.

### Step5
<br>
Predict the CO2 emission of the car where the weight is 2300kg,and volume is 1300cm cube.

### Step6

Print the predicted output. 
 
## Program:
```
# NAME : Jeyabalan
# REG NO :212222240040
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
print("Predicted Co2 for the corresponding weight and volume",predictedCO2)

```
## Output:
![image](https://github.com/jeyaqbalan7/Multivariate-Linear-Regression/assets/119393851/aa8d1c2f-3a3d-4058-93c6-e1423fb889eb)


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
