# Day 17
Today we have studied about git and git branching and then installed jupyter in Ubuntu and now learning supervised learning
## Supervised Machine Learning
*   
*   We need a DataSet for training
*   Then we give this data to system for training for learning purpose
*   Then the training model is ready for QnA.
*   Then we give a new question related to the training model.
*   Example
    *   When we see a dog for the first time, someone introduce us that this object is a dog. Similarly when we see another breed of a dog or an animal we can identify that which animal it is.
*   The actual object is called as ```label```
*   The attributes | Features | Characterstics of an object are ```features``` for computer.
*   So we have to give both label and its features to the system for training purpose.
*   Model Data
    *   Apple
        *   Texture : Smooth
        *   Weight  : 100-120 Grams
    *   Orange
        *   Texture : Bumpy
        *   Weight  : 120-140 Grams
```py
# Here Smoooth is for apple and Bumpy is for Orange
features=[[100,"Smooth"],[120,"Smooth"],[130,"Bumpy"],[150,"Bumpy"]]

label = ['apple','apple','orange','orange']
```
*   Now we need an algorithm for training purpose.
*   Supervised Machine Learning
    *   Classifier This means when we need to distinguish between features and attributes or basically classifying data<br>
    Data Classifiers techniques for Supervised Learning
        *   KNN
        *   SVM
        *   Decision Tree
        *   Naive Bagos
        *   Random Foresh
        *   Lion
        *   Me
    *   Regression will discuss later for this.
*   In python there is a liberary called scikit which contains all the above classifiers. It is a framework containing all the classifiers written in python.
*   Since by default we dont have ```scikit-learn``` installed so we have to install it with pip3
```
pip3 install scikit-learn
```
*   Since we only need the package ```tree``` from sklearn as such we will import
```py
from sklearn.tree import DecisionTreeClassifier
```
*   To Train our model we need some questions and answers, Here the questions are called as features and answers are called as labels.
```py
# Here Smoooth is for apple and Bumpy is for Orange
    # Smooth = 0
    # Bumpy = 1
features=[[100,0],[120,0],[130,1],[150,1]]
label = ['apple','apple','orange','orange']
```
*   Now in order to put this data we need a classifier and we will use Decision Tree Classifier for this.
```py
# Calling Decision Tree Classifier
clf = DecisionTreeClassifier()
```
*   There is a function in the classifier called ```fit``` which is used to fit the features and labels in the Algorithm in order to train it for results.
```py
# Now time for Training data
trained = clf.fit(features,label)
```
*   Now the variable ```trained``` is the brain of our program and it will be used to predict the queries.
*   Now we will use the ```predict``` function in order to predict the data by entering a question and it will return an answer for that.
```py
# Now time for pridicting
trained.predict([[110,0]])
array(['apple'], dtype='<U6')

trained.predict([[123,1]])
array(['apple'], dtype='<U6')

trained.predict([[119,1]])
array(['apple'], dtype='<U6')
```
*   Since now we are able to predict the data by the trained variable and it results us the desired output.

