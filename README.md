# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.import the required packages.
2.Import the dataset to operate on.
3.Split the dataset.
4.Predict the required output.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Yuvan M
RegisterNumber:  212223240188
import chardet
file='/content/spam.csv'
with open(file,'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result


import pandas as pd
data=pd.read_csv('/content/spam.csv',encoding='Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values
y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
### data.head()
![image](https://github.com/Yuvan291205/Implementation-of-SVM-For-Spam-Mail-Detection/assets/138849170/54d69ece-e020-49de-8fc5-4d758bd5d723)
### data.info()
![image](https://github.com/Yuvan291205/Implementation-of-SVM-For-Spam-Mail-Detection/assets/138849170/5e18f690-72f7-4083-92f1-94e1cb95e857)
### data.isnull().isum()
![image](https://github.com/Yuvan291205/Implementation-of-SVM-For-Spam-Mail-Detection/assets/138849170/e0408d9f-546f-482f-bcf3-9b00e31e2f61)
### y pred:
![image](https://github.com/Yuvan291205/Implementation-of-SVM-For-Spam-Mail-Detection/assets/138849170/da6cf15d-4403-46f2-8c0e-c8847be14821)
### accuracy:
![image](https://github.com/Yuvan291205/Implementation-of-SVM-For-Spam-Mail-Detection/assets/138849170/f70f52ca-3b19-4298-a3ce-028769afcc73)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
