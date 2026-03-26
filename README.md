# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Open new file in jupiter notebook.

### Step2
Import the neccessary libraries and load the data.

### Step3
Define input (Volume, Weight) and output (CO2)

### Step4
Create regression model

### Step5
Predict for new input

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:

![alt text](<Screenshot 2026-03-26 141810.png>)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.