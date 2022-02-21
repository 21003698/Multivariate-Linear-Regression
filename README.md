# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import panda

### Step2
import linear mode; from sklearn

### Step3
Read the file cars.csv


### Step4
Assign the values for x and y as required



### Step5
Create the linearRegression model and predict the output


## Program:
~~~
#Developed by :- challa sandeep
#Register number:- 212221240011
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)


~~~
## Output:
<img width="802" alt="Screenshot 2022-02-21 at 8 39 12 PM" src="https://user-images.githubusercontent.com/93427522/154982627-b8644868-f27d-4b89-80b0-d887358ff2e4.png">



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
