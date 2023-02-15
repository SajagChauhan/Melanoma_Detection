# Melanoma_Detection


## Table of Contents
* [Problem Statement](#problem-statement)
* [General_Information](#General-Information)
* [Approach Used](#Approach-used)
* [Observations & Results](#observations-&-results)



## Problem Statement
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## General_Information
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

### Images pertaining to diseases:
 ![Screenshot 2023-02-15 122652](https://user-images.githubusercontent.com/86041805/218954867-21c31d5a-fd07-489a-b45f-a1ff820a8a53.png)



## Approach Used
- Understanding the data.
- Create train & validation datasetwith batch size of 32 with resizing images to 180*180.
- Perform Data Visualization
- Build model while scaling image to normalize pixel value between (0,1).
- Choose loss function and optimizer for model training and train it for 20 epochs.
- check whether the model underfit or overfit.

![overfit](https://user-images.githubusercontent.com/86041805/218956312-6c7ee7f9-f17a-40d4-9eb1-bc56592f3e1a.png)

As you can see the model overfits.
- Now we use a proper Augmentation technique to overcome overfitting issue.
- Training the model again and checking if it perform better or not.

![augmentation](https://user-images.githubusercontent.com/86041805/218956949-fceb0abc-9224-4e87-ab24-a36a8bf83d08.png)

- Check for Class distribution 

![class imbalance](https://user-images.githubusercontent.com/86041805/218957819-766cdd9a-4de1-4cf4-abc2-c05ff6a35e80.png)

- Using augmentor library to handle class imbalances.
- Train the model on the data created using Augmentor using 50 epochs.

![final model](https://user-images.githubusercontent.com/86041805/218958509-ef0742e6-f581-41b0-b8bd-7c3709a5dc1a.png)



## Observations & Results
From the above Analysis, We conclude that: 
The results are comparatively better than the previous model.The problem of overfitting and underfitting has been addressed to an extent very carefully. The accuracy of Validation and Training has been improved and same happens for the Training Loss and Validation Loss.

![final](https://user-images.githubusercontent.com/86041805/218959140-f9db258a-5674-4f8f-b655-d167e26907cd.png)

![accur](https://user-images.githubusercontent.com/86041805/218959638-57ebfce8-0b17-4887-bf3a-2ffb2d328885.png)




## Contact
Created by [@SajagChauhan] - feel free to contact me!
