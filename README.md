## EEG dataset to classify alcoholic & non-alcoholic persons

This project aims to recognize the person as either alcoholic or non-alcoholic based on their EEG sample data

<!-- 
<img src= "https://i.ibb.co/x8tXZK0/alcoholic.gif">

<img src = "https://i.ibb.co/QXDwNKK/control.gif"> -->

We began with some set of textual data which was collected from multiple people and classified as Alcoholic and Controlled

This dataset was extracted from the zip files and converted into csv format for each person

The dataset was then cleaned and converted into excel format for removing noise using Matlab

Then the multiple files for each person were combined into a single excel file 

We then used a method called FORce which is used to remove all the artifacts from the dataset which is basically non-human noise data in the EEG signal

The next steps to be followed will be feature extraction using discrete wavelet transform and applying a classifier to the dataset
