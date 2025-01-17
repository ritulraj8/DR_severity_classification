Diabetic Retinopathy Classification using ResNet18
This repository contains code for classifying diabetic retinopathy severity using a pre-trained ResNet18 model. The model is trained on the Diabetic Retinopathy dataset and achieves an accuracy of%.

Dataset
The Diabetic Retinopathy dataset used in this project can be found(/kaggle/input/diabetic-retinopathy-dataset). It contains images of retinal scans classified into five categories:

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
Class: Healthy,Precision: 99.36, Recall: 97.98
Class: Mild DR,Precision: 86.19, Recall: 95.67
Class: Moderate DR,Precision: 99.10, Recall: 91.66
Class: Proliferative DR,Precision: 94.27, Recall: 92.64
Class: Severe DR,Precision: 80.21, Recall: 98.72
