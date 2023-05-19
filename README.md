# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Varsha.G
RegisterNumber:  212222230166
import pandas as pd
data=pd.read_csv("Employee.csv")

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
1. data.head()

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/127f6116-fc9a-4bc0-94e7-bf6ed07f5663)

2. data.info()

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/5cec3286-c21c-465d-a88c-cdd5a4582c0d)



3. isnull() and sum()

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/9fcb425a-c537-4f19-886f-5087faa732eb)


4. data value counts()

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/bcd926af-f0a8-4c09-b168-18839cee678a)


5. data.head() for salary

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/56a0bda4-ed4a-4983-a006-2d6812c0d332)


6. x.head()

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/4ea71a06-66fb-47f3-89e8-d16db5472b1e)


7. accuracy value

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/5f31f3a2-8ae8-4987-bf34-18e16a12023a)

8. data prediction

![image](https://github.com/varsha-2005/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119288183/f973beca-eec6-4435-861e-c2ecd08b32c8)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
