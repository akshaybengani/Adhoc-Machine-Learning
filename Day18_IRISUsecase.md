# Day 18

In previous class we learned about Decision Tree Classifier and we have installed Scikit Learn.

## Decision Tree Classifier
*   It remembers its output
*   It is a classifier not an algorithm
*   The Algorithm which runs in background is ID3 and CART.
*   It makes different cases and checks the features of objects one by one.
*   Out of all features Decision Tree selects one feature as head node and checks all possible circumstances.
*   GraphVizier graph wizard is used or can be to findout which feature is placed on top of Decision Tree.
*   We can use Cancer prediction by Decision Tree
*   The more features | Attributes much better decision tree will develop
*   It can be used for house price prediction by more data and attributes like location, size, nearby searvices and enviorment etc etc.
*   We can use it for Text recorgination and number shapes prediction.
*   Decision Tree supports regression.
## DataSets
So now we will learn about DataSets. It is a huge package of resources and classes of sample data and solutions, here you just need to use the existing liberaries in order to perform a certian task.
*   To import datasets from sklearn use
```py
from sklearn import datasets
import time
```
*   Now we will list all the datasets functions and classes.
```py
for i in dir(datasets):
    print(i)
    time.sleep(1)
```
*   Since the classes starting from ```load``` are the datasets we will be using.
```py
[i for i in dir(datasets) if 'load' in i]
```
## IRIS
*   We will now learn about ```IRIS```. It is a flower which is found in ireland which is used for making medicines.
*   University of Califonia used 3 categories of it for medicine research.
    *   Setosa
    *   Versicolor
    *   Virginica
*   Features | Attributes of Flower
    1.  Sepel Length
    2.  Sepel Width
    3.  Petal Length
    4.  Petal Width
*   Now we need to load iris data from sklearn
*   There are sub packages or classes in the iris package.
```py
from sklearn.datasets import load_iris
iris = load_iris()
dir(iris)

['DESCR', 'data', 'feature_names', 'filename', 'target', 'target_names']
```
*   To read description of IRIS use
```py
print(iris.DESCR)
```
*   To read about its features use
```py
print(iris.feature_names)
```
*   The data of Features | Questions | Attributes is stored in iris.data
```
iris.data
```
*   To get shape of the data
*   The data is 150 rows and 4 columns means 150 examples in 4 different categories.
```
actualData = iris.data
actualData.shape
(150, 4)
```
*   The actualData variable is numpyArray
*   Now we have seen the features and attributes and data inside it now its time to check the answers or labels of all 150 records.
```
iris.target
```
*   



