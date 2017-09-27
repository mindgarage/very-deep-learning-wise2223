# 2. Programming Tasks

## Prerequisites
1. **Keras:** [https://keras.io/](https://keras.io/)
2. **Python:** 2.7+

## 2.1 Build a Convolutional Neural Network

This task is meant to get you acquainted with one of the Deep Learning frameworks called Keras.
The main goal of this task is to build a simple Convolutional Neural Network and train it on the MNIST dataset.

### Task Description
**Convolutional Neural Networks** (Conv Nets, a.k.a. CNNs) have led to a paradigm shift in the field of Computer Vision.
While popular Conv Net architectures (e.g., Alex Net, LeNet, ResNet, etc.) are generally used in vision problems directly,
 we still need to come up with our own architectures to deal with very specific problems.

### Part 1
For this part of the task you need to develop the following Conv Net architecture using Keras:

#### Layers

**1. Conv Layer:** num_filters=64,  kernel_size=(3, 3), activation=relu, padding=valid, strides=(2, 2)

**2. Conv Layer:** num_filters=32,  kernel_size=(2, 2), activation=relu, padding=same, strides=(1, 1)

**3. Max Pool Layer:** pool_size=(2, 2)

**4. Dropout:** rate=0.35 (Fraction of the input units to drop)

**5. Flatten**

**6. Dense:** num_units=256, activation=tanh

**7. Dropout:** rate=0.5 (Fraction of the input units to drop)

**8. Dense:** num_units=10, activation=softmax

### Part 2

Train the above architecture on the MNIST dataset with the following optimizers for 10 epochs each and plot 
their corresponding loss curves.

Use **categorical Cross Entropy** as the loss function.

#### Optimizers

1. Adam
2. ADADELTA
3. Stochastic Gradient Descent

#### Resources
1. [Keras CNN MNIST Example](https://github.com/fchollet/keras/blob/master/examples/mnist_cnn.py)
2. [Keras Optimizers](https://keras.io/optimizers/)


## 2.2 Popular Architectures and Fine Tuning

This task will make you familiar with some popular Conv Net architectures, which are:
**1. ResNet**
**2. InceptionV3**

Along with that, you will get a first hand experience on finetuning Deep Learning models.

### Task Description
Train a **ResNet** and an **InceptionV3 Net** on a dataset of **Cats and Dogs** 
(can be found [here](https://www.kaggle.com/c/dogs-vs-cats/data)). Submit your Mean Error Rates and Accuracies.

### Task Requirements

1. Create **3 stratified splits** with ration **7:2:1** (train, validation and test)
2. train the models and report the **Accuracies** and **Mean Error Rates** for both the models.
3. Use **Binary Cross Entropy** as the loss function

#### Resources
Thanks to Keras, you will not have to develop everything from scratch. You can use pretrained models that Keras provides 
and finetune them with your datasets.

1. [Keras Applications](https://keras.io/applications/)
2. [Stratification](http://scikit-learn.org/stable/modules/generated/sklearn.model_selection.StratifiedKFold.html)

# References
...
