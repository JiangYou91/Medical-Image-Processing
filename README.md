# Brain Tumors MRI Images Segmentation CNN(AE)+LSTM
##Introduction
The goal of this work is to reimplement the CNN based LSTM, a model which takes in the same time the spatial and temporal information. This design aims to improve the performance of 3D Brain tumors MRI images segementation. In particular, a set of brain slicing image could be considered as a sereis of moving image.

## Method
This experiments compare the result of segementation with Autoencoder, CNNbased LSTM, and its variation, Bidirectional CNN-LSTM. As a basical design, the model is composed of 3 part: 1. CNN based encoder, 2. LSTM Layers, 3. CNN based decoder.

The model takes a series of MRI images of type T2 as input, and gives the shape of tumors on a background. The loss function is MSE for comparing two images.

The set are split into 2 parts, 70% for training and 30% for test.

## Result
The current result shows that the Unet with LSTMCon2d layers could perform better than the original Unet. The following table represents the Dice score of lesion of four levels. It shows that the Dice score are improved in the 3 level except that in 1 level it has been slightly reduced.

