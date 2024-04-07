# Classification with Neural Networks

## Overview

This repository contains a Python script to classify fashion images using a neural network. The Fashion MNIST dataset is used, which consists of 60,000 training images and 10,000 testing images across 10 different fashion categories.

## Requirements

- tensorflow
- matplotlib

Install the required packages using pip:

```bash
pip install tensorflow matplotlib
```

## Data Loading and Exploration

The Fashion MNIST dataset is loaded using TensorFlow's built-in `fashion_mnist` dataset. The dataset is split into training and testing sets, and an example image with its corresponding label is displayed using matplotlib.

## Data Preprocessing

The pixel values of the images are normalized to the range [0, 1] by dividing by 255.0. Additionally, a validation set is created by taking the first 5000 samples from the training dataset.

## Building a Neural Network Architecture

A neural network model is constructed using TensorFlow's Keras API. The model consists of three layers: 

1. Flatten layer to convert 2D input images (28x28 pixels) into 1D arrays.
2. Dense layer with 300 neurons and ReLU activation function.
3. Dense layer with 100 neurons and ReLU activation function.
4. Output Dense layer with 10 neurons (one for each class) and softmax activation function.

## Model Compilation and Training

The model is compiled with the sparse categorical crossentropy loss function, SGD optimizer, and accuracy metric. It is then trained on the training dataset for 30 epochs, with validation data provided for monitoring the model's performance during training.

## Prediction

The trained model is used to make predictions on the first 5 test images. The predicted class probabilities are printed, and the predicted classes (i.e., the classes with the highest probabilities) are determined using `argmax`.

## Conclusion

This project demonstrates how to build, train, and evaluate a neural network for image classification using the Fashion MNIST dataset. The model achieves decent accuracy on the validation set and can be further optimized by tuning hyperparameters, adding more layers, or using advanced techniques like data augmentation.

##images
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/0be613f1-e742-483f-b7b4-e28cfe758284)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/476a5159-12a3-44f2-a97e-721863a82bb2)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/759adf8a-629d-4a4d-ae6b-6d33ea43b121)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/ac93e65e-6327-470c-8718-75081c1e0de2)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/9fcdb679-5dfb-4bef-9265-846012a9d51b)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/1f08ff22-04e1-4395-97d6-0d21d0680340)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/6d8b8540-9b77-4203-b66b-707694d92f1b)
![image](https://github.com/AISHWARYAAU/classification-with-Neural-Networks/assets/91381783/3f902b0b-24a1-4769-b1af-8900cd658467)







