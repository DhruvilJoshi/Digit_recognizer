# Digit_recognizer

•	Preprocessing dataset:
The data has 280 images divided in 10 folders 0-9. Those are also its classes. I resize those images to (28,28), also convert it to grayscale and store it as a list. I also scale pixel intensities to the range [0, 1]. The dataset is divided into 80% for training and the remaining 20% for testing.

•	Model training:
I use a LeNet model structure. It is a convolutional neural network structure proposed by Yann LeCun et al. in 1989. It is very simple and for our dataset seem to be good enough. It has 2 Convolution layers, 1 Fully connected layer and 1 Softmax classifier. I calculate loss using categorical_crossentropy and I use a adam optimizer. I train the network for 25 epochs as it starts to overfit if I continue.

•	Results:
The loss at final epoch is of 0.4040, the accuracy is at 0.8884, the validation loss is of 0.9569 and the validation accuracy is at 0.7. Further I could train on MNIST or similar dataset and test it on our dataset.
