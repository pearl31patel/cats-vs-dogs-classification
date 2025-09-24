This project is a Convolutional Neural Network (CNN) built with TensorFlow & Keras to classify images of dogs and cats.
The dataset comes from Kaggle’s Dogs vs Cats dataset.


Training set: 20,000 images (cats and dogs)
Validation/Test set: 12,461 images (cats and dogs)


**Labels**
0 → Cat
1 → Dog


**CNN Architecture**
The Convolutional Neural Network (CNN) used in this project is built with four convolutional blocks followed by fully connected layers. The first block starts with 32 filters, then the second, third, and fourth blocks use 64, 128, and 256 filters respectively. Each block consists of a convolution layer with a ReLU activation, followed by batch normalization and max pooling to reduce spatial dimensions and improve generalization. After flattening the feature maps, the network includes two dense layers with 128 and 64 units, each followed by dropout for regularization. Finally, a single dense output layer with a sigmoid activation function is used to classify the input image as either a cat (0) or a dog (1) .


**Final Results**
Training Accuracy: 97.54%
Training Loss: 0.0667
Validation Accuracy: 89.96%
Validation Loss: 0.3824
( The model shows strong performance on training data and good generalization to validation data. )


**Summary**
The CNN can successfully distinguish between cats and dogs with ~98% training accuracy and ~90% validation accuracy.
