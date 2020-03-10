# Ground Control Point (GCP) Marker Classification module for python 

A convolutional neural network pretrained on MNIST dataset was used. The
final layer with 10 classes was replaced with a layer having two output
classes. Accuracy is about 93%. (accuracy depends on the type of images used for classification, proper preprocessing will give you a good accuracy).

(network architecture:
https://github.com/keras-team/keras/blob/master/examples/mnist_cnn.py)

Class 1: Marker

Class 2: Non Marker

 ## How to use: 

-   Clone this repository to your local working directory.

-   First run setup.sh file in your Linux machine ( \$bash setup.sh)

-   This will install the required dependencies such as tensorflow and
    Keras. You might want to check before if you have installed these
    two (tensorflow and Keras) already. Because it may cause conflict
    between different versions. Create a different enviroment if this happens.

-   Now you can import classifier module using import statement (import
    classifier). Instantiate a classifier object and then use classify
    method for classifying images. Make sure the images are of the
    specified dimensions (28 \* 28).

-   The output of classify method is a numpy array containing the predicted 
    probability of two classes

## Examples of positive and negative classes:

Positives: (class 1) check in class1 directory

Negatives: (class 2) check in class2 directory

This module is not be used as a standalone detector.
