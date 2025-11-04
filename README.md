# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
STEP 1 - Start

STEP 2 - attach the given data file

STEP 3 - now find the satisfaction level of employee data

STEP 4 - find the accuracy and new predict value

STEP 5 - Stop

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: JAYAVARSHA T
RegisterNumber: 212223040075

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]]) 
*/
```

## Output:
<img width="1128" height="223" alt="Screenshot 2025-11-04 152235" src="https://github.com/user-attachments/assets/3319bf7e-f383-4139-a258-7bc57b04ce2c" />

<img width="577" height="127" alt="Screenshot 2025-11-04 152313" src="https://github.com/user-attachments/assets/690aed31-a267-4193-839a-74281d1a2bd1" />



<img width="360" height="116" alt="Screenshot 2025-11-04 152433" src="https://github.com/user-attachments/assets/e8a15933-72bf-4dcf-b936-08c2887f9045" />


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
