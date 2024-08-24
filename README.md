# Image Classifier Web App

This project is a web application that classifies images into one of ten categories using a pre-trained neural network model. The app is built with [Taipy](https://taipy.io/), a GUI framework, and utilizes a TensorFlow Keras model for image classification.

## Features

- **Image Classification**: Upload an image to classify it into one of the following categories:
  - Airplane
  - Automobile
  - Bird
  - Cat
  - Deer
  - Dog
  - Frog
  - Horse
  - Ship
  - Truck

- **Image Display**: View the uploaded image along with the classification result.

- **Probability Indicator**: See the classification probability of the image.

## How It Works

1. **Model Loading**: The app loads a pre-trained TensorFlow Keras model (`baseline.keras`), which has been trained to classify images into one of ten predefined categories.

2. **Image Processing**: When an image is uploaded, the app processes the image by:
   - Opening and converting it to RGB.
   - Resizing it to 32x32 pixels.
   - Normalizing pixel values to the range [0, 1].

3. **Prediction**: The processed image is passed to the model to predict the class. The app then displays:
   - The classification result.
   - The probability of the predicted class.

4. **User Interface**: The application interface is built using Taipy, which provides a simple file selector for uploading images and displays the results in a user-friendly format.
