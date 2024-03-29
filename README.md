Machine-Learning Resources 💻🚀
===============================

Contents
--------
**[`Naive Bayes`](#naive-bayes)__,__[`Support Vector Machine`](#support-vector-machine)__,__[`Boolean`](#boolean)__,__[`Lists`](#lists)__,__[`Dictionaries`](#dictionaries)__,__ [`Tuples`](#tuples)__,__[`Sets`](#sets)__,__[`None`](#none)**  

Naive Bayes
--------
**Refer to Udacity: Intro to Machine Learning and for code and understanding refer link below**
* https://www.geeksforgeeks.org/naive-bayes-classifiers/

example:
```python
# load the iris dataset 
# the Iris dataset will generate data to play with
from sklearn.datasets import load_iris 
iris = load_iris() 
  
# store the feature matrix (X) and response vector (y) 
X = iris.data 
y = iris.target 
  
# splitting X and y into training and testing sets
# train_test_split generates test data and training data
from sklearn.model_selection import train_test_split 
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.4, random_state=1) 
  
# training the model on training set 
from sklearn.naive_bayes import GaussianNB 
gnb = GaussianNB() 
gnb.fit(X_train, y_train) 
  
# making predictions on the testing set 
y_pred = gnb.predict(X_test) 
  
# comparing actual response values (y_test) with predicted response values (y_pred) 
from sklearn import metrics 
print("Gaussian Naive Bayes model accuracy(in %):", metrics.accuracy_score(y_test, y_pred)*100)
```

Support Vector Machine
--------
**Refer to Udacity: Intro to Machine Learning and for code and understanding refer link below**
* **https://www.geeksforgeeks.org/classifying-data-using-support-vector-machinessvms-in-python/**

Code Example:
```python
# import support vector classifier 
from sklearn.svm import SVC # "Support Vector Classifier" 
clf = SVC(kernel='linear') 
  
# fitting x samples and y classes 
clf.fit(x, y)
```
