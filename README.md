# 18xd28-facial-expresion-analysis-and-emotional-classification
A simple attempt to classify faces based on emotion. Part of 18xd28 course under AMCS at PSG college of technology. By 19PD29 

## How to use

#### The Model
The trained model and data set used is present in the repository. The model can directly be used into any appropriate applicatio. A sample implementation, for testing the model, is provided in app.py. 

Please make sure the neccessary libraries are present (in requirements.txt file)

The data is a ck+ dataset taken from https://www.kaggle.com/shawon10/ckplus

It is slightly modified as per the needs.

#### app.py
```
Install the required libraries into a virtual environment
Create a directory called test in the same directory as the app.py
Place images into the directory
Run app.py 
The results will be in a folder called temp in the same directory
```
The app can identify the faces in the test folder. Its pretty straight forward to use.
It draws a box over the identified face and labels the predicted emotion. 

## How it works
It is a simple deep learning model using the keras library. The comments in the ipython notebook give a brief overview of the steps. It is a Sequential model from Keras. It has a simple architecture with 2 convolutional layers, one dense hidden layer and an output layer.

Increasing the amount of data can improve the performance significantly, but it will also increase the computational demand.
