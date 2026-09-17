Deep Learning – Fashion Image Classification

Project Overview

This project demonstrates how Deep Learning can be used to classify fashion product images into different product categories.

The project uses the Fashion MNIST dataset and a simple Artificial Neural Network (ANN) built with TensorFlow/Keras. The model learns patterns from labelled fashion images and predicts the category of unseen images.

Business Problem

In an e-commerce business, employees may need to manually identify and categorize thousands of product images before listing them online.

This project demonstrates an AI-assisted approach where a Deep Learning model can analyze a product image and predict its category, reducing repetitive manual work.

Example Process

Product Image → Deep Learning Model → Predicted Product Category → Human Review (if required)

Dataset

The project uses the Fashion MNIST dataset, which contains grayscale images of fashion products.

The 10 categories are:

T-shirt/Top

Trouser

Pullover

Dress

Coat

Sandal

Shirt

Sneaker

Bag

Ankle Boot

The dataset is loaded directly through TensorFlow/Keras, so no manual dataset upload is required.

Technologies Used

Python

TensorFlow / Keras

NumPy

Matplotlib

Google Colab

Artificial Neural Network (ANN)

Deep Learning

Model Architecture

The notebook uses a simple neural network:

Input Image (28 × 28)
        ↓
Flatten
        ↓
Dense Layer – 64 neurons
        ↓
ReLU Activation
        ↓
Dense Layer – 10 neurons
        ↓
Softmax
        ↓
Predicted Fashion Category

Training Configuration

Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Metric: Accuracy

Epochs: 3

Validation Split: 10%

Data Preprocessing

The original pixel values range from 0 to 255.

They are normalized to values between 0 and 1 by dividing the images by 255.0. This prepares the image data for the neural network.

Prediction

After training, the model:

Evaluates its performance on test images.

Predicts the category of an unseen image.

Compares the predicted category with the actual category.

Displays the image along with the prediction.

Business Benefits

A similar system could help an e-commerce company with:

Faster product listing

Reduced repetitive manual work

More consistent product categorization

Improved product-search experience

Processing a larger number of product images

Limitations

The model's predictions are not always correct. Accuracy alone may not be sufficient for business deployment because incorrect categorization can affect customer experience and product discovery.

Human review can remain important, especially for uncertain or high-impact classifications.

Project Structure

Deep_Learning_Fashion_Image_Classification/
│
├── Deep_Learning_Fashion_Classification_Abhay_Trehan.ipynb
└── README.md

How to Run

Open the notebook in Google Colab or Jupyter Notebook.

Run the cells from top to bottom.

TensorFlow automatically downloads the Fashion MNIST dataset.

Train the model for 3 epochs.

Check the test accuracy.

Try different image_number values to test additional predictions.

Learning Outcomes

This practical demonstrates:

How images can be used as Deep Learning input.

The basic structure of an Artificial Neural Network.

The role of input, hidden and output layers.

Image normalization.

Model training and testing.

Classification using Softmax probabilities.

Connecting an AI/ML model with an e-commerce business use case.

Academic Context

Course Area: Artificial Intelligence / Machine Learning
Topic: Deep Learning – Image Classification
Program: BBA FinTech
Student: Abhay Trehan

Key Takeaway

Deep Learning can automate repetitive image-classification tasks, but businesses should consider model accuracy, data quality, classification risk, and human oversight before deploying such systems.
