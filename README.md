# Multiclass classification model using a custom convolutional neural network in Tensorflow.
To build a ***CNN based model*** which can accurately ***detect melanoma***. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

### Problem Solution
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the ***International Skin Imaging Collaboration (ISIC)***. All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

1. Actinic keratosis
2. Basal cell carcinoma
3. Dermatofibroma
4. Melanoma
5. Nevus
6. Pigmented benign keratosis
7. Seborrheic keratosis
8. Squamous cell carcinoma
9. Vascular lesion
 

### Project Pipeline

***Data Reading/Data Understanding:*** 
 - Defining the path for train and test images

***Dataset Creation:*** 
 - Create train & validation dataset from the train directory with a batch size of 32. 
 - Resize images to 180*180.

***Dataset visualisation:*** 
 - Create a code to visualize one instance of all the nine classes present in the dataset 
 - Model Building & training : 
 
   1. Create a CNN model, which can accurately detect 9 classes present in the dataset. 
   2. While building the model rescale images to normalize pixel values between (0,1).
   3. Choose an appropriate optimiser and loss function for model training
   4. Train the model for ~20 epochs
   5. Write your findings after the model fit, see if there is evidence of model overfit or underfit

***Choose an appropriate data augmentation strategy to resolve underfitting/overfitting***

***Model Building & training on the augmented data :***
 - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
 - Choose an appropriate optimiser and loss function for model training
 - Train the model for ~20 epochs

***Class distribution:***
 - Examine the current class distribution in the training dataset 

***Handling class imbalances:***
 - Rectify class imbalances present in the training dataset with Augmentor library.

***Model Building & training on the rectified class imbalance data :***
 - Create a CNN model, which can accurately detect 9 classes present in the dataset. 
 - While building the model rescale images to normalize pixel values between (0,1).
 - Choose an appropriate optimiser and loss function for model training
 - Train the model for ~30 epochs
 
