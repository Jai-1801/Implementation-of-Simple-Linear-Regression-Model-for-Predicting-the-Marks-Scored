# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard Libraries.
2.Set variables for assigning dataset values.
3.Import linear regression from sklearn.
4.Assign the points for representing in the graph.
5.Predict the regression for marks by using the representation of the graph.
6.Compare the graphs and hence we obtained the linear regression for the given datas. 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: JAI SURYA.R
RegisterNumber:  212223230084

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.metrics import mean_absolute_error, mean_squared_error


df=pd.read_csv("student_scores.csv")
print("Dataset :")
print(df)
print()
print("Head Values :\n",df.head())
print("Tail Values :\n",df.tail())
print()
X=df.iloc[:,:-1].values
Y=df.iloc[:,1].values
print("X_Values :\n",X)
print()
print("Y_Values :\n",Y)
print()


from sklearn.model_selection import train_test_split
X_train,X_test,Y_train,Y_test=train_test_split(X,Y,test_size=1/3,random_state=0)


from sklearn.linear_model import LinearRegression
regressor=LinearRegression()
regressor.fit(X_train,Y_train)
Y_pred=regressor.predict(X_test)


print("Y_prediction Values : \n",Y_pred)
print("\nY_test Values : \n",Y_test)


print()

print("Training Set Graph :")
plt.scatter(X_train,Y_train,color="purple")
plt.plot(X_train,regressor.predict(X_train),color="darkblue")
plt.title("Hours vs Scores (Training Set) ")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()


print()

print("Test Set Graph :")
plt.scatter(X_test,Y_test,color="darkgreen")
plt.plot(X_test,regressor.predict(X_test),color="lightgreen")
plt.title("Hours vs Scores (Test Set) ")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()

print()


print("Values for MSE, MAE, & RMSE :")
MSE=mean_squared_error(Y_test,Y_pred)
print("MSE = ",MSE)
MAE=mean_absolute_error(Y_test,Y_pred)
print("MAE = ",MAE)
RMSE=np.sqrt(MSE)
print("RMSE = ",RMSE)
*/
```

## Output:
![306719591-c1c8a803-9293-4d66-9d37-ac29bea29249](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/6ec522a6-8e95-4f2e-ad2d-87e4e2b67842)

![306719602-c4ffc740-ee23-4328-b2c4-1fffaba0ee38](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/c493ebf3-31e6-461e-91bf-d0a2848194e3)

![306719627-feddc9e1-1b4d-4d9f-8ac5-9d65856ef656](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/f0b61692-8880-4284-881a-10f4f667b581)

![306719647-f8e03823-6767-41df-9662-da0bb429abc8](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/09148ed0-7bc0-4ec7-bb51-a8a1ee604ab1)

![306719679-38c5ba65-cd06-449c-b737-83617acc2c5b](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/fd8e9b97-b365-467c-b5e9-710a41129897)

![306719693-cca18e3b-b700-4a1f-a184-92c2b3cb4d3f](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/de93d671-6047-412b-a93d-869fadda0550)

![306719724-f2c4adbc-c098-42ac-91da-a37b70d161cf](https://github.com/Jai-1801/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/139335300/08a4a24f-f9d2-4c1c-a266-041c252f7a97)




## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
