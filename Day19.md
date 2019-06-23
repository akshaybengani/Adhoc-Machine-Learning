# Day 19
*   Today we will learn about ```KNN``` Classifier.
```KNN``` is called as K Nearest Neighbour.
*   KNN will work on Ecludien Distance algorihm.
*   KNN will not work efficiently when we have a large datasets.
*   KNN will calculate distance from each point and then sort in nearest points.
*   KNN groups it near by points.
*   It is recommended to take the KNN value as odd number and dont take 1.
*   KNN supports regression.
## KNN in IRIS DataSets.
```py
# Loading iris dataset
from sklearn.datasets import load_iris
# Loading in a variable
iris = load_iris
# Display classes of iris package
dir(iris)
# Display the Target Names or Answers
iris.target_names
# Display Features Name or Questions
iris.feature_names
```
## Regression
*   It is used when we have to predict Stock Price, Cricket Run, Salary, Study models.
*   Example Data for study and marks
    *   4 hours study
    *   2 eat
    *   7 sleep
    *   Marks are 67%
*   Categories in Regression
    *   Linear Regression when we get straight line its linear
        *   y = Mx + b
        *   Salary = Experience x Factor + b
        *   b is the coefficient 
    *   Ploynomial Regression when we increase by squares in equation.
### Tasks
*   Design a UI in Html asking a button ```upload```.
*   The file it will accept is JSON CSV or EXCEL
*   When upload completes it will show the data in form of tables using pandas.
*   It will ask from a dropdown regarding which algorithm to use
*   It will then ask for testing data percentage again in options menu
*   If the classifier is KNN then it should ask for K value
*   After clicking submit it will show a graph plotting the data either on bar Scatter pie ask from user at that point or in previous page.




