# Traffic Recognition Machine Learning Program Documentation

## Introduction

This Python program is designed to effectively identify and categorize traffic signs depicted in images using convolutional neural networks (CNNs). By employing state-of-the-art deep learning techniques, it facilitates the automated recognition and classification of diverse traffic sign variants.

## Installation

To get started, make sure you have Python installed on your system. Then, install the necessary dependencies by running:

```bash
pip install tensorflow numpy opencv-python-headless matplotlib scikit-learn
```
These dependencies include TensorFlow for machine learning, NumPy for number crunching, OpenCV for image processing, Matplotlib for visualizing data, and scikit-learn for data prep and evaluation.

# Usage
## 1. Data Preparation
First things first, gather your dataset. Collect images of different traffic signs and organize them into directories, each representing a specific sign category. Make sure your images are in the .ppm format for compatibility.

## 2. Loading Data
Next up, load your dataset using the **load_data** function. Don't forget to specify parameters like the image dimensions (**IMG_WIDTH** and **IMG_HEIGHT**) and the total number of sign categories (**NUM_CATEGORIES**). This function will give you back a handy tuple with all your loaded images and their corresponding labels.

## 3. Data Preprocessing
Before diving into model training, let's prep our data. Split it into training, cross-validation, and test sets using scikit-learn's **train_test_split** function. Oh, and don't forget to reshape those images to the right dimensions!

## 4. Model Creation
Time to build the CNN model! I'm using TensorFlow.keras's **Sequential** API here. Define your model architecture, including the input layer, hidden layers, and output layer. Tweak the number of neurons and activation functions to suit your needs.

## 5. Model Training
With our model architecture in place, let's train it! Compile the model by picking an optimizer, loss function, and evaluation metric. Then, train it using the training data and keep an eye on its performance using the cross-validation data. Feel free to tweak those hyperparameters to get the best results!

## 6. Model Evaluation
Once training is done, it's time to see how our model performs. Evaluate its performance using the test data. Plotting accuracy and loss curves can give us a good visual on how our model is doing and whether it's overfitting or underfitting.

## Results
Running the program will give you some cool metrics like loss and accuracy. Visualizing the training and validation loss, as well as the model's accuracy, will help you understand how well your model is doing.

## Conclusion
My Traffic Recognition Machine Learning Program is a game-changer in the world of transportation systems. By harnessing the power of CNNs and advanced machine learning techniques, I've created a tool that can accurately classify traffic signs, contributing to safer and more efficient roads.

## License
This program is distributed under the MIT License, so feel free to tweak it and share it as you see fit.

## Author
[Evan Harlan](https://github.com/EvanHarlan)
