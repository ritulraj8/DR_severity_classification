Diabetic Retinopathy Classification using ResNet18

This repository contains code for classifying diabetic retinopathy severity using a pre-trained ResNet18 model. The model is trained on the Diabetic Retinopathy dataset and achieves an accuracy of 95%.

Dataset

The Diabetic Retinopathy dataset used in this project can be found at /kaggle/input/diabetic-retinopathy-dataset. It contains images of retinal scans classified into five categories:

Healthy
Mild DR
Moderate DR
Proliferative DR
Severe DR


A pre-trained ResNet18 model from torchvision.models is used for this task. The final fully connected layer of the model is modified to output 10 classes. The model is trained using the Adam optimizer and cross-entropy loss function.

Usage
To run the code, make sure you have the following libraries installed:

torch
torchvision
matplotlib
numpy
PIL
sklearn
seaborn
You can then run the main.py script to train and evaluate the model.

Results
The model achieves an accuracy of 95% on the test set. The precision and recall for each class are as follows:

Class	  Precision	Recall
Healthy	 99.36%	  97.98%
Mild DR	 86.19%	  95.67%
Moderate 
DR	     99.10%	  91.66%
Proliferative 
DR	     94.27%	  92.64%
Severe 
DR	     80.21%	98.72%

A confusion matrix heatmap is also generated to visualize the model's performance.


