# Skin Cancer Abnormality Classification 
## Machine learning Model used - Convolution Neural Networks

### Goal
Train a Convolution Neural Networks model to predict and classify the type of skin cancer from any given :file_folder: image.

### Dataset 
Source : https://www.isic-archive.com/#!/onlyHeaderTop/gallery

Size of dataset :file_folder: was 49.9 Gigabytes, our systems could handle only 1500 images at a time during training.
So this project was stored, processed and run on an Amazon EC2-P2 instance. 

### Quick info
Quick Link for Code: https://github.com/yuvaraja402/Skin-Cancer-Convolution-Neural-Networks/blob/master/Skin_cancer_CNN_notebook.ipynb

Jupyter Notebook was used for code developement in Python.

Output snapshots are stored under 'Outputs Snapshots' folder.
Post the training, 10 images :file_folder: were selected to validate classifying accuracy with the trained model. They are stored in the folder 'Single prediction images'.

### Workflow
Setup:

As local computer :computer: will be inefficient during model's training time from images, this project was run on Amazon EC2-P2 instance for faster training and results.
P2 instance was powered by Nvidia Tesla K80 GPU to power up the project. 

Technologies used:

Python :snake: code as base for processing and training from images.
P2 instance was connected with Jupyter notebook for easier interaction.
Keras package in python with Tensorflow as Backend for creating Convolution, Pooling and Dense layers to train the images and get started with prediction.

Project flow:

Established the connnection of Jupyter notebook on P2 instance for easy interaction with the cloud service during development. Developed python script using Keras package to process images that were stored in the cloud using WinSCP tool. During training and testing the project ran as a single script to avoid delays. This same project when run on a laptop :computer: with Nvidia GTX 1050Ti took ~1 hour 20 minutes to completely train the image dataset whereas in P2 instance :computer: with Nvidia K80 GPU it took only 20 minutes. The purpose of using Cloud service was to minimize training time and increase output quality.

Neural Network details:

* Convolution layers - 2
* Feature maps - 32 in first batch and 64 in later batch 
* Pooling layers - 2
* Hidden layers - 2 (each has 128 neurons)


Instance details :computer: :

* GPU - Nvidia Tesla K80
* vCPU's - 4
* Ram - 61 (GiB)
* Network bandwidth - High
* Price/hour - $0.900

### Result :tada:
Prediction accuracy :bar_chart: of the model is 81.47 %.

In real world test of 8/10 images were accurately predicted :white_check_mark:.

As future scope, this model can be trained with more samples to reach metrics :chart_with_upwards_trend: of 95 %.
