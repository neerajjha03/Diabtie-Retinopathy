# Diabtie-RetinopathyDiabetic Retinopathy Classifier and Web App
 https://retinopathy-classifier.herokuapp.com
Details
The following were used for model training (see requirements.txt):

fastai: version 1.0.52
PyTorch: version 1.0.0
Python: version 3.6
A SqueezeNet pretrained on the ImageNet dataset was used to train the classifier.

Training was done with Kaggle Kernels. Training history is provided in history.csv

The dataset came from the Diabetic Retinopathy Kaggle Competition, with the files cropped to remove any black space, and resized to a width of 1024 (and maintaining the aspect ratio), before being loaded in fastai.

The following were used for model deployment:

Heroku (Free Dyno)
Flask: version 1.0.2
gunicorn
The dataset was hosted in Kaggle Datasets. Model progress (monitored by CSVLogger Callback in fastai) and saved models (saved by the SaveModelCallback in fastai) were outputted by the kernel.

xudates Segmentation in Fundus Images
In this project, we apply Image morphology & Clustering to get candidates for exudates pixels. Finally a SVM classifier is applied to get segmentation results.

Getting Started
These instructions will get you a copy of the project up and running on your local machine for you to test the algorithms on your own fundus images. The DIARETDB1 database has been used for demonstration here for which we are grateful.

Bloodvessel Segmentation
Check a subsection at BLOOD VESSEL SEGMENTATION

Prerequisites
The following must be installed and configured:

Python
Opencv
Sample Output
For some image in DIARETDB1:



Following resultant images are produced while segmentation process (different candidates for single profile of fundus):














