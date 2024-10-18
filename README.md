# Image-Classification
This project implements an image classification model using TensorFlow and Keras. The model is designed to classify images of animals into multiple categories (e.g., antelope, cat, dog, etc.) using a Convolutional Neural Network (CNN).

Features
Data Splitting: Automatically splits a dataset of images into training, validation, and test sets using splitfolders.
Convolutional Neural Network (CNN): The model is built using Keras with several layers of convolutions and pooling to extract features from images.
Data Augmentation: Resizes and normalizes images for efficient model training.
Model Training and Evaluation: Trains the model on the training set, validates it on the validation set, and evaluates performance using accuracy and loss metrics.
Prediction: After training, the model predicts the class of a new image with its confidence score.
Model Saving: The trained model is saved for future use.
Workflow
Data Preparation:

Images are organized into directories, each representing a class.
The dataset is split into training, validation, and test sets with a 70/20/10 ratio.
Model Training:

A CNN is trained on the training data and validated on the validation data. The model uses three convolutional layers with pooling and dropout for regularization.
Training and validation accuracy/loss are tracked across multiple epochs (25 in this case).
Model Evaluation:

The model’s performance is visualized using plots for accuracy and loss for both training and validation data.
Predictions are made for test images to check the model's ability to classify unseen data.
Image Prediction:

You can load an image, process it, and get a predicted class with a confidence score.
Installation
Clone the repository:

git clone https://github.com/username/repo-name.git
cd repo-name
Install the required Python packages:

pip install tensorflow split-folders numpy pandas matplotlib
Set up your dataset:

Ensure your dataset is stored in the appropriate directory structure, where each class has its own folder of images.
Update the paths in the code to match the locations of your dataset.
Run the code to split the dataset and train the model.

Usage
Splitting the Dataset:

import splitfolders
splitfolders.ratio(input_folder, output=output_folder, seed=38, ratio=(.7, .2, .1))
Model Training:
Train the model on your dataset.
Track performance across 25 epochs.

