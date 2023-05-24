# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas as pd
2. Obtain the information of data.
3.Get the sum of null values.  
4. Print the MSE value.
5.Print the R^2 value.
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: 
RegisterNumber:

**
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
**
**
data.head()
**
**
data.info()
**
**
data.isnull().sum()
**
**
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
**
**
data["Position"]=le.fit_transform(data["Position"])
data.head()
**
**
x=data[["Position","Level"]]
y=data[["Salary"]]
**
**
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
**
**
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
**
**
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
**
**
r2=metrics.r2_score(y_test,y_pred)
r2
**
**
dt.predict([[5,6]])
*/
```

## Output:
![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/6502ce4a-f539-4cb7-b2a2-7a3fe2ba248c)

![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/206fd001-f939-4798-8730-4fa5721f4c7b)

![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/726a56f7-10a4-44c2-8eed-f3e6d0ab2b8b)

![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/4f4528b0-d874-4ead-8c77-e116b15abeed)

![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/a9fd2b22-47e0-4a55-b958-31bc8a4f83e9)

![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/dad28f21-d890-4670-962b-bd3379bb7563)

![image](https://github.com/Meetha22003992/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119401038/e0cd877d-0c79-4a1a-b426-4db1c672d16a)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
