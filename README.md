# CNN_Classification
A basic image classification project using Convolutional Neural Networks (CNN) with TensorFlow and Keras. The model is trained to classify images into two categories: cats and dogs.
This project implements an image classification model using a Convolutional Neural Network (CNN) with TensorFlow and Keras. The model is trained to classify images into two categories: cat and dog.

First, the training and testing data are loaded from CSV files using NumPy. The input data represents images, while the labels represent their corresponding classes. The data is reshaped into the format (100, 100, 3) so that it can be processed as color images. The pixel values are normalized by dividing by 255 to improve model performance.

A random image from the training dataset is displayed using Matplotlib to visually verify the data.

The CNN model is built using the Sequential API. It consists of convolution layers to extract features from images, max pooling layers to reduce image size, and fully connected layers for classification. The final output layer uses a sigmoid activation function since this is a binary classification problem.

The model is compiled using the Adam optimizer and binary cross-entropy loss. It is trained on the training data for 5 epochs and then evaluated on the test dataset to measure accuracy. After training, the model is saved for future use.

Finally, a random test image is selected and passed to the trained model for prediction. Based on the prediction value, the image is classified as either a cat or a dog, and the result is printed.
