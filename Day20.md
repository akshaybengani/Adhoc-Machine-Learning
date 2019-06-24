# Day 20 Data enginnering
* A classifier requires an accurate data to use its processing algorithm
* Pre processing of data before applying ML is know as Data Engineering
*   Steps
    *   Clean
    *   Recycle
    *   Auto Fill
*   Pandas is very similar to SQL. It basicallyy creates its own format called as DataFrame.
*   To describe your data like count,min,max,avg,mean etc.
```py
df.describe()

	Age	Salary
count	9.000000	9.000000
mean	38.777778	63777.777778
std	7.693793	12265.579662
min	27.000000	48000.000000
25%	35.000000	54000.000000
50%	38.000000	61000.000000
75%	44.000000	72000.000000
max	50.000000	83000.000000
```
*   If we want to fix missing values or replacing missing value with some releveant data then we have to use a liberary from SciKit Learn.
```py
from sklearn.preprocessing import Imputer
```
*   
*   
*   
*   Data Processing have a branch called Dummy Variable.


