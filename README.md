# UPF-DL-2020

This github is about to present the code of our final project, which title is Early Exits on Convolutional Neural Networks.


## Introduction
This project focuses on CNN and its ability to classify images among different labels, but we do not focus on how much 
accuracy we can get by implementing some different CNN design models. Our principal concern is about the weakness of 
overthinking in deep neural networks. Overthinking means that the network is able to correctly classify images before the 
final layers. Overthinking problem involves computational waste, and there could also be the case where a correct prediction 
at some internal layer in the network turns out in a misclassification when it reaches the output layer.


## Data and model used.
For such analysis, we decided to use CIFAR-10 dataset. This dataset consists of a 10-label classification dataset which 
includes 60000 input images, 6000 images per layer. The dataset is divided into 50000 labeled images used for training (train 
set), and 10000 images for testing (test set). The following image shows the different labels and some sample images in the 
dataset.

![alt text](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/1_sGochNLZ-qfesdyjadgXNw.png)

So, once introduced the dataset let's talk about our model. In fact, we created two different type of models using ResNet18.
- 2-Exits model. We created a model with 1 early exit and the output/final exit.
- 3-Exits model. We created a model with 2 early exits and the output/final exit.

In this github there is provided the code to run both models (to perform train and test operations).
The code to train 3 Exits model is 'EE_cifar10_training-3exits.ipynb', and 'EE_cifar10_test_3exits.ipynb' for testing.
'EE_cifar10_training_2exits.ipynb', and 'EE_cifar10_test_2exits.ipynb' are to run 2 Exits implemented model.

In each model, you will also see there is the possibility to train data using different pooling techniques (Average pooling or 
Spatial Pyramid Pooling). In order to try one or other model, you just need to modify the cell where the function is called.
(You will encounter better results when using Spatial Pyramid Pooling).

'' file is implemented in order to display obtained results, principally comparing our early exit implementations with the original ResNet18 model.



## Results
In order to ease the testing of our project, we provide the following links, which directly redirects to a public collab with clear instructions on how to try the previously explained different models.

Links to colab: 
- 2 Exits model: https://drive.google.com/file/d/1uZyNDiSinVed_efMfYCW_egfmSr1gzUy/view?usp=sharing
- 3 Exits model: https://drive.google.com/file/d/1MvA-TX4J4bjdH6E1dST_dz_Y1Jor7Wtd/view?usp=sharing
_________
Marcelo Sanchez, Raul Rivas & Aleix Pujol.
Universitat Pompeu Fabra.
