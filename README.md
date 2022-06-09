# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
#step:
Import pandas module and import the required data set.
#step:
Find the null values and count them.
#step3:
Count number of left values.
#step4:
From sklearn import LabelEncoder to convert string values to numerical values.
#step5:
From sklearn.model_selection import train_test_split
#step6:
Assign the train dataset and test dataset.
#step7:
From sklearn.tree import DecisionTreeClassifier.
#step8:
Use criteria as entropy.
#step9:
From sklearn import metrics.
#step10:
Find the accuracy of our model and predict the require values


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by:k.sucharitha 
RegisterNumber:212221240021

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level",	"last_evaluation",	"number_project",	"average_montly_hours",	"time_spend_company",	"Work_accident","promotion_last_5years","salary"]]
x.head()
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
![5 1](https://user-images.githubusercontent.com/94166007/172895842-41dd97dd-b985-4a29-a155-6d5f8cea4005.jpeg)
![5 2](https://user-images.githubusercontent.com/94166007/172895897-efa04af7-2435-4d8b-9c9f-d943392cfc14.jpeg)
![5 3](https://user-images.githubusercontent.com/94166007/172895917-bf558a00-16d3-4fd9-bb7e-73eec7ebb24a.jpeg)
![5 4](https://user-images.githubusercontent.com/94166007/172895923-6973cab5-bfa6-4dd8-9f53-f03c0742f535.jpeg)
![5 5](https://user-images.githubusercontent.com/94166007/172895935-b8aaa888-e3e6-4395-b181-664a9ae3cb82.jpeg)
![5 6](https://user-images.githubusercontent.com/94166007/172895975-ca2c383b-6ab3-4175-964e-f2bc84a6b4d9.jpeg)
![5 7](https://user-images.githubusercontent.com/94166007/172895996-eaddfac4-500e-43c7-a8e0-29632e81dc0a.jpeg)
![5 8](https://user-images.githubusercontent.com/94166007/172896011-cddc612a-787f-4893-8571-63f426226151.jpeg)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
