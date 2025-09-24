CIFAR-10 Image Classification with Deep Learning

1.Problem Statement Image classification is a fundamental task in computer vision where the goal is to categorize images into predefined classes. This project focuses on classifying the CIFAR-10 dataset, which contains 60,000 images across 10 categories such as airplanes, cars, birds, cats, and more.

2.Deep Learning Methods & Description

Fully Connected Neural Network (Dense Layers)

The network uses multiple dense layers to process flattened image pixel data.

Dropout layers are applied to prevent overfitting.

Different initializers and regularizers can be tested for optimization.

Activation Function (ReLU)

Introduces non-linearity to help the network learn complex patterns.

Dropout Regularization

Randomly disables neurons during training to reduce overfitting.

3.DL Methods Applied to Solve the Problem

Data Preprocessing

Normalized image pixel values to the range [0, 1]. Converted labels to one-hot encoded vectors. Model Architecture

Input: Flattened 32×32×3 images. Dense layer with 512 neurons + ReLU activation. Dropout (0.3) for regularization. Dense layer with 256 neurons + ReLU activation. Output layer with 10 neurons (softmax) for classification. Training

Dataset: CIFAR-10 training set. Loss: Categorical cross-entropy. Optimizer: Adam. Evaluation on CIFAR-10 test set.

4.Results Achieved a good accuracy test set. Successfully classified images into 10 categories. Visualized sample predictions to confirm model learning.

5.Conclusion This project demonstrates a simple yet effective approach for CIFAR-10 classification using dense neural networks. Although convolutional neural networks (CNNs) could improve performance, this architecture shows how dense layers can still capture patterns in image data after flattening.
