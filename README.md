# Project Write-Up
## Overview of Assignment
This assignment is working on the fruits dataset with 90380 images of 131 fruits and vegetables. The purpose of the project is to address the classification task which will train a model that can classify input image data according to given 131 classes. 
## Description of data
The dataset consists of 3 folders of fruits and vegetable images: Training, Test, test_multiple_fruit. 
The images in the 3rd folders are images with combination or mixes of many types of fruits while the images in Training and Test folders are one fruit or vegetable in each image. So, this assignment only focus on dataset in the 2 folders 'Traing', and 'Test'.
<li>The total number of images: 90483.
<li>
Training set size: 67692 images (one fruit or vegetable per image).
<li>
Test set size: 22688 images (one fruit or vegetable per image).
<li>
The number of classes: 131 (fruits and vegetables).
<li>Image size: 100x100 pixels </li>

## Summary of methods
Firstly, in the preprocessing step, the dataset was normalized. The 'Training' dataset was used to train the model and splitted into 'training set' and 'validation' set with 80:20 ratio. 
Then, 3 models were built to address the multiclass classification task.
## Summary of model
The base CNN model consisted of 3 convolutional layers, two with 32 filters and one with 64 filters. I also added MaxPooling, and BatchNormalization layers for each convolution layers. This model was fit with normalized dataset and performed 85% accuracy. <br>
Next, I applied Data Augementation techniques into the Normalization step to see the improvement. In addition, I increased the number of epochs from 15 to 25.</br>
## Analysis of results
The base model performed pretty well and the data augementation technique hasn't contributed significantly. However, the accuracy score was improved from 85% to 87,6%. 

## Conclusion and potential future work
This project to classify fruits and vegetable can benefit in many fields such as health care, retails, etc. For example, these kinds of classification model can help a supermarket cashier quickly scan and recognize type of fruits that benefit for a quick check-out. <br> The potential high accuracy score may be contributed by the hard work of building and collecting data about fruits and vegetables.</br>
Some of future work could be explored in an effort to improve the model:
<li> Explore more options of factors such as number of epochs, epochs steps, etc. or other ways of data augementation to optimize model performance.
<li> Try other pretrained model such as xception, ResNet, etc.
