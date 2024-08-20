# PRODIGY_ML_03

This project involves implementing a Support Vector Machine (SVM) model to classify images of cats and dogs using a dataset from Kaggle. Here's a brief overview of the steps involved:

Project Overview
Dataset Access:

The dataset is accessed directly from Kaggle. It contains images of cats and dogs, with each image labeled accordingly. There is no need to manually unzip the dataset.
Image Preprocessing:

Loading Images: The images are loaded from the directory using OpenCV.
Resizing: Each image is resized to a consistent size (e.g., 64x64 pixels) to ensure uniform input for the model.
Normalization: Pixel values are normalized to a range of 0 to 1 by dividing by 255. This helps in improving model performance and convergence.
Data Preparation:

Flattening Images: Images are converted from 2D arrays (height x width x channels) into 1D arrays (flattened) because SVM models require 1D feature vectors.
Feature Scaling: Features are standardized using StandardScaler to improve the performance of the SVM.
Model Training:

An SVM classifier with an RBF (Radial Basis Function) kernel is trained on the flattened, scaled image data. The RBF kernel is used to handle non-linear relationships in the data.
Model Evaluation:

Predictions: The trained model makes predictions on a separate test set.
Accuracy: The accuracy of the model is calculated to assess how well it classifies the test images.
Classification Report: A detailed report showing precision, recall, and F1-score for each class (cat and dog) is generated.
Confusion Matrix: A confusion matrix is plotted to visualize the performance of the classifier, showing the number of true positives, false positives, true negatives, and false negatives.
Model Saving:

The trained model is optionally saved to a file for future use or deployment.
Summary
The project leverages SVM, a powerful classification algorithm, to distinguish between images of cats and dogs. It involves preprocessing images, converting them into a suitable format for SVM, training the model, evaluating its performance, and optionally saving the trained model. The approach combines image processing techniques with machine learning to build an effective image classifier.
