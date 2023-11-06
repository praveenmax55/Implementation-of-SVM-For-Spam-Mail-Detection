# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.  Import the required packages.
2.  Import the dataset to operate on.
3.  Split the dataset.
4. Predict the required output.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Praveen D
RegisterNumber: 212222240076

import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extractiaon.text import CountVectorizer
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

Data Head:

![173846588-8b6564a7-5154-4768-8392-d7e73101f989](https://github.com/Naveensrinivasan07/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119475891/98cf9f3c-90e5-41e5-8084-437f8a7a9540)

Data Info:

![173846683-02ba0f71-d91f-4b25-bfd0-567c99c1a53f](https://github.com/Naveensrinivasan07/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119475891/2a7fe9fe-467e-49d0-b290-00aaeb796c83)

Data isnull():

![173846738-9177ccfc-1f83-41e6-829f-45970c7ad578](https://github.com/Naveensrinivasan07/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119475891/9a6b632d-fdae-41a1-a5cd-d9417422c871)

y_pred:

![173846832-fe73c991-28a1-44e1-9397-fc7bdff02b88](https://github.com/Naveensrinivasan07/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119475891/dab0af6d-6757-4713-a501-47c1f173d523)

Accuracy:

![173846885-378f6ef8-4913-4bd1-a146-7a72d0c72d19](https://github.com/Naveensrinivasan07/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119475891/407969be-056e-4b50-98d8-c070f1265ba4)



## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
