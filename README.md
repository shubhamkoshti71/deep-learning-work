# Assignment - Deep Learning Practice

Practice training a deep neural network on the CIFAR10 image dataset:

1. Build a DNN with 20 hidden layers of 100 neurons each (that’s too many, but it’s the point of this exercise). Use He initialization and the Swish activation function.
2. Using early stopping, train the network on the CIFAR10 dataset. You can load it with `tf.keras.datasets.cifar10.load_data()`. The dataset is composed of 60,000 32 × 32–pixel color images (50,000 for training, 10,000 for testing) with 10 classes, so you’ll need a softmax output layer with 10 neurons. Remember to search for the right learning rate each time you change the model’s architecture or hyperparameters.
3. Now try adding Batch Normalization and compare the learning curves: is it converging faster than before? Does it produce a better model? How does it affect training speed?
4. Try replacing Batch Normalization with SELU, and make the necessary adjustments to ensure the network self- normalizes (i.e., standardize the input features, use LeCun normal initialization, make sure the DNN contains only a sequence of dense layers, etc.).  How does the performance change?
