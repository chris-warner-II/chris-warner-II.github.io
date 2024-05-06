---
title: "Assorted PyTorch portfolio projects (Personal Project)"
excerpt: "<img src='/images/pytorch.jpg' width='500' height='400'> <img src='/images/jupyter.png' width='250' height='250'> <br/> This portfolio contains a number of machine learning projects in PyTorch demonstrate ability to implement algorithms in that domain. They range from topics like regression to binary and multiclass classification to computer vision to creating custom datasets to transfer learning with pretrained models. This is a *growing* repository and I am currently working to add example projects focusing on Transformers, RNNs, LSTMs, speech recongnition using CNNs and spectrograms, etc."
collection: portfolio
---

Skills & Expertise:
------
machine learning, pytorch, regression, binary classification, multiclass classification, computer vision, CNN, transfer learning, 



Though I have been steeped in deep/machine learning due to pursuing my Ph.D. in computational neuroscience during its rise (2011-2019), my specific projects focused on other topics within neuroscience and data modelling. While I am quite comfortable with neural networks on a conceptual and academic level, I have not coded up many neural network algorithms ... until now! This [repo](https://github.com/chris-warner-II/pytorch_projects) contains a *growing* number of projects implemented in PyTorch and showcased in Jupyter Notebooks that demonstrate my ability to develop machine learning algorithms. 

Finished projects include:
------

1. [`01_Linear_Regression.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/01_Linear_Regression.ipynb) - implements linear regression on linear and non-linear data with 1-layer linear NN, 3-layer linear NN model and 3-layer nonlinear NN model
2. [`02_Binary_Classification.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/02_Binary_Classification.ipynb) - implements binary classification on some 2-class datasets that are not linearly separable
3. [`03_Multi_Classification.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/03_Multi_Classification.ipynb) - implements multiclass classification on some datasets that are and are not linearly separable using 3-layer linear and nonlinear neural networks
4. [`04_Computer_Vision_FashionMNIST.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/04_Computer_Vision_FashionMNIST.ipynb) - explores FashionMNIST dataset to do multiclass classification using linear, non-linear networks and finally using a CNN architecture
5. [`04b_Computer_Vision_CIFAR.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/04b_Computer_Vision_CIFAR.ipynb) - performs multiclass classification on CIFAR dataset using a CNN architecture.
6. [`05_Custom_Datasets.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/05_Custom_Datasets.ipynb) - building a custom dataset to train CNN model to perform food classification, exploring data augmentation
7. [`06_VGG_imagenette_Transfer_Learning.ipynb`](https://github.com/chris-warner-II/pytorch_projects/blob/main/06_VGG_imagenette_Transfer_Learning.ipynb) - building a custom dataset and dataloader out of imagenette dataset, training a CNN model from scratch, as well as finetuning a torchvision pretrained model on new dataset

Continuing progress:
------
1. `Transformer_model.ipynb` - work through tutorial implementing a Transformer model
2. `RNN_model.ipynb` - work through tutorial implementing a RNN model
3. `LSTM_model.ipynb` - work through tutorial implementing a LSTM model
4. `Autoencoder_model.ipynb` - work through tutorial implementing a Autoencoder (and VAE) model
8. `Phoneme_Classifier_CNN_TIMIT.ipynb` - build a multiclass classifier for phonemes based on spectrograms of phonemes in the TIMIT dataset
9. `Next_Letter_Prediction.ipynb` - build next token prediction model for letters using RNN, LSTM and Transformer models using torchtext for dataset
10. `Next_Phoneme_Prediction.ipynb` - build next token prediction model for phonmemes using RNN, LSTM and Transformer models using torchtext for dataset and CMUDict to convert word to phonemes.


