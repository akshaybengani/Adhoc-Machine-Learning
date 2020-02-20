# Day 34
* CANN Convolutional Artificial Neural Network.
* Three keywords for CANN
    *   Convolution
    *   Max Pooling
    *   Flattening
*   Convolution means the matrix of 3x3 which shifts along the image matrix and then creates a feature map as a new image.
*   Max pooling means collecting all the largest numbers in window and create a new matrix.
*   Flattening means adding up the previous matrix in single dimensional matrix.
*   Over fitting is basically a problem which arise due to training model again and again which leads to changing data which leads to decrease in accuracy of the model is called overfitting.
*  Command to check RAM Slot
```
sudo dmidecode -t 17 | grep -i size
```