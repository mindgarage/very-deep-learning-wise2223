# 2. Programming Tasks

## 2.1 Popular Architectures and Fine Tuning

This task will make you familiar with some popular Conv Net architectures, which are:
**1. ResNet**
**2. InceptionV3**

Along with that, you will get a first-hand experience on finetuning Deep Learning models.

### Task Description
Train a **ResNet** and an **InceptionV3 Net** on a dataset of **Cats and Dogs** 
(can be found [here](https://www.kaggle.com/c/dogs-vs-cats/data)). Submit your Mean Error Rates and Accuracies.

### Task Requirements

1. Create **3 stratified splits** with ration **7:2:1** (train, validation and test)
2. train the models and report the **Accuracies** and **Mean Error Rates** for both the models.
3. Use **Binary Cross Entropy** as the loss function

#### Resources
Thanks to Keras, you will not have to develop everything from scratch. You can use pre-trained models that Keras provides and finetune them with your datasets.

1. [Keras Applications](https://keras.io/applications/)
2. [Stratification](http://scikit-learn.org/stable/modules/generated/sklearn.model_selection.StratifiedKFold.html)

# References
...
