## Classification of Alcoholics & Non-Alcoholics via EEG signals

This project aims to recognize the person as either alcoholic or non-alcoholic based on their EEG sample data

<!-- 
<img src= "https://i.ibb.co/x8tXZK0/alcoholic.gif">

<img src = "https://i.ibb.co/QXDwNKK/control.gif"> -->

## Data cleaning

We began with some set of textual data which was collected from multiple people and classified as Alcoholic and Controlled

This dataset was extracted from the zip files and converted into csv format for each person

The dataset was then cleaned and converted into excel format for removing noise using Matlab

Then the multiple files for each person were combined into a single excel file 

We then used a method called FORCe which is used to remove all the artifacts from the dataset which is basically non-human noise data in the EEG signal


## Feature extraction

Feature extraction using the discrete wavelet transform function was applied to each of the files for ```15``` epochs, where each epoch was of ```4``` seconds and sampling rate was ```256``` Hz.

Post creation of wavelet transform variables over the whole dataset for 15 epochs, we began feature extraction for each of the features

The following features were extracted :
* Wavelet energy
* Shannon entropy
* Mean
* Variance
* Median

The average value of each feature was taken over the 15 epochs for each wavelet coefficient.

<img src = "https://i.ibb.co/yNn82w7/Screenshot-2023-04-06-233611.png">


The data was then converted to ```5(features) * 6(wavelet coefficients) = 30``` columns for classification

## Classification
