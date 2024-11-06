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
data=pd.read_csv("spam.csv",encoding='Windows-1252')
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

![Screenshot 2024-11-06 112924](https://github.com/user-attachments/assets/c0abafbd-70e0-4441-a051-5a22db0835c6)


Data Info:

![Screenshot 2024-11-06 112933](https://github.com/user-attachments/assets/7b2834fa-8c68-4481-a01a-481ad7fe9cf5)


Data isnull():

![Screenshot 2024-11-06 112946](https://github.com/user-attachments/assets/6b6fc687-d124-4840-b4c0-ae2ff250acc3)


y_pred:

![Screenshot 2024-11-06 112758](https://github.com/user-attachments/assets/cad45e98-7bb2-46f6-994d-762243562043)


Accuracy:

![Screenshot 2024-11-06 112806](https://github.com/user-attachments/assets/12367a47-4043-447b-832f-ca5d7a51b317)




## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
