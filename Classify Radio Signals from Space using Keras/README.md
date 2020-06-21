# Classify-Radio-Signals
Classify Radio Signals - 2D Spectrograms into 4 Categories ( Squiggle, Narrowband, Noise and Narrowbanddrd) using Convolutional Neural Network.

## Dataset
This is a 2D Spectrogram image data of Radio Signals. Initially, it was initially a time-series data, captured by SETI(Search for extraterrestrial intelligence) institute, which was later converted to 2D Spectogram image data. The 2D Spectogram enables us to treat this as a image-classification problem.

The dataset can be downloaded from https://drive.google.com/drive/folders/1FaDxc0yEh7T7mY1v1LEOS4NoUs2mu7pJ?usp=sharing .

### Processing
* Keras ImageDataGenerator function is used as a data generator function.
* Image Augmentation of Horizontal Flip is used.

## Model
This project uses **3 Convolutional Networks** (With Batch Normalization, Activation Function Relu and Dropout Regularization) , **1 Dense Layer** with Dropout and the **4-class Output Layer** with Softmax Activaion.

### Learning Rate
To increase the convergence with gettin accurate results, Keras **Exponential Decay Function** is used. 

## Results
The model aquires **75.13%** accuracy on the validation set.

Graph of the Loss and Accuracy over epoch :
![Loss and Accuracy](files/Loss_accuracy.png)
