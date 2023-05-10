# Melanoma_Detection

## General Information
- Multiclass classification model using a custom convolutional neural network in TensorFlow. 

- Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

## Table of Contents
* Data Reading/Data Understanding
* Dataset Creation
* Dataset visualisation
* Model Building & training
* Model Building & training on the augmented data
* Class distribution
* Handling class imbalances
* Model Building & training on the rectified class imbalance data

## Conclusions
* Model 1:-
- The model is overfitting
- Loss and accuracy of train and validation is almost equal at 4th and 5th epcoh
- The accuracy is around 90% and validation accuracy is 49% because there are enough features to remember the pattern.
- Loss is very high
* Model 2:- (augmented data)
- Model is still under fitting but better then first model.
- But the accuracy of train is just about 49% and validation is around 48%
- Loss seems to be more now.
* Model 3:- (After handling class imbalance and using regularization)
- The class rebalance helped in reducing overfititng of the data and thus the loss is beng reduced But the Acurracy very low
- Initially we tried without the ImageDataGenerator which created data to over fit.
- Then we introduced dropout and ImageDataGenerator which reduced the over fit
- At last we tried Batch Normalization and Augumentation which helps in reducing overfitting and loss.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - version 3.10.11
- Tensorflow - version 2.12.0
- Keras - version 2.12.0
- Augmentor - version 0.2.12

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->
