CIFAR-10 Classification with Fully Connected Neural Network

1.Problem Statement The goal of this project is to classify images from the CIFAR-10 dataset into ten different categories using a fully connected (Dense) neural network architecture. CIFAR-10 is a widely used benchmark dataset in computer vision, consisting of 60,000 32x32 color images in 10 classes, with 6,000 images per class.

2.Deep Learning Methods Used Dense (Fully Connected) Neural Network: The model uses a sequential architecture with multiple dense layers to learn representations from image data.

Layers Included: Flatten layer to convert image matrices into 1D arrays. Two Dense layers with 128 and 68 neurons respectively, activated by ReLU. Output Dense layer with 10 neurons (one for each class), activated by softmax.

3.Method Description Preprocessing:

Input images are normalized to the range. Labels are one-hot encoded for multi-class classification. Model Compilation: Optimizer: Adam Loss Function: Categorical Crossentropy Metrics: Accuracy

Training: 10 epochs Batch size: 32 20% of the data is used for validation during training.

4.Results Test Accuracy: The final test accuracy (on the unseen test data) is printed after evaluation.

Learning Curves: Training and validation loss and accuracy are plotted to visualize performance over epochs.

5.Conclusion This project demonstrates how a simple fully connected neural network can be applied to the CIFAR-10 image classification problem. Although convolutional neural networks (CNNs) are more commonly used for image classification, this model achieves reasonable performance and illustrates the workflow from data preparation to evaluation using Keras and TensorFlow.
