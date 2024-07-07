# Project Name
> Melanoma Detection Assignment


# Author
> Dipak Sah
 
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
In this assignment, we are building a multiclass classification model using a custom convolutional neural network in TensorFlow. 

Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

We are provided with dump of the dataset. 

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion
 
Important NOTE:

We are not using any pre-trained model using Transfer learning. All the model building processes are based on a custom model.
It is advised to use GPU runtime in Google Colab due to large no of epochs.

## Conclusions
### - Conclusion : Model with input train data without dropout
        1.  Accuracy:  0.91796875 and Validation Accuracy:  0.48769575357437134
        2.  The difference in accuracy between training and validation accuracy is very significant which is a sign of overfitting.

### - Conclusion : Model with input train data with dropout
        1.  Accuracy:  0.8404017686843872 and Validation Accuracy:  0.5212528109550476
        2.  Both training accuracy and validation accuracy has declined a little. But, the difference in accuracy between training and validation accuracy still very significant which is a sign of overfitting.

### - Conclusion : Model with data augmentation applied in keras sequential
        1.  Accuracy:  0.5452008843421936 and Validation Accuracy:  0.5145413875579834
        2.  Overfitting is handled but accuracy delined drastically below 54%.

### - Conclusion : Model with class imbalance rectified with Augmentor Library, also applied batch normalization
        1.  Accuracy:  0.8312314748764038 and Validation Accuracy:  0.7037861943244934
        2.  After balacing the dataset, we do not see any sign of overfitting or underfitting.


## Technologies Used
- Tensor Flow Version : 2.15.0
- Pandas Version      : 2.0.3
- Numpy  Version      : 1.25.2
- Seaborn Version     : 0.13.1
- Augmentor Version   : 0.2.12


## Acknowledgements
Give credit here.
- This project is guided by Tanisha Medewala , out teacher from Upgrad.
- This project is dedicated to all my co-learners from ML C60 batch.


## Contact
Created by [@dipaksah20] - feel free to contact me!


