# Skin Cancer Abnormality Classification 
# Model - Convolution Neural Networks

Project - 4 people project

### Dataset 
Source : https://isic-archive.com/#images

Size of dataset was 49.9GB, out of which our systems could handle only approx 1500 images since Epoch times for training the images took
 tremendous time.

### Code
Link : https://github.com/yuvaraja402/Skin-Cancer-Convolution-Neural-Networks/blob/master/Skin_cancer_CNN_3.ipynb

Jupyter Notebook was used for code developement in Python. 

### Goal
The goal was to train the Convolution Neural Networks so it could detect type of cancer in skin from any given new image.

### Method
Used Keras package with Tensorflow as Backend for creating Convolution, Pooling and Dense layers to train the images and get started with prediction.

Convolution layers - 2,Feature maps - 32 in first batch adn 64 in next batch, Pooling layers -2 and Hidden layers - 2 (each has 128 neurons)

GPU - Nvidia GTX 1050 Ti was utitlized for computing the convolution and neural network layers. 
### Result
After prediction, validation accuracy was 81.47 %.
We single predicted with 10 images, out of which 8 turned out to be accurate so giving us 80% accuracy.

In future, the same model can be trained with larger image dataset in a machine thats capable of handling the workload.
