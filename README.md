# Brain Tumor Detection with VGG-16 CNN Transfer Learning

Aim of the project is to use Computer Vision techniques of Deep Learning to correctly detect Brain Tumor for assistance in Robotic Surgery.

Here, I build a Convolutional Neural Network (CNN) model that would classify if subject has a tumor or not based on MRI scan. We have used VGG-16 model architecture and weights to train the model for this binary classification problem. The following MRI Scans have no tumor while those given later have Brain Tumor. 

<p align="center">
    <img width="700" height="300" src = 'https://github.com/aviralchharia/Brain-Tumor-Segmentation-with-Deep-Neural-Networks/blob/main/Images/No%20Tumor.png?raw=true'
</p>

<p align="center">
    <img width="700" height="300" src = 'https://github.com/aviralchharia/Brain-Tumor-Segmentation-with-Deep-Neural-Networks/blob/main/Images/Tumor.png?raw=true'
</p>

But to use these images in our Deep Learning Model, we need to pre-process these images first. Data Augmenation is also performed to increase the size of the training data as we make use of limited data. The images are cropped as shown in the Figure below.

<p align="center">
    <img width="750" height="200" src = 'https://github.com/aviralchharia/Brain-Tumor-Segmentation-with-Deep-Neural-Networks/blob/main/Images/Data%20Preprocessing.png?raw=true'
</p>

Using the CNN Model to classify the MRI Scans into Tumor & Non-Tumor classes, we obtain the following Model Accuracy & Loss Curves. The confusion matrix for the Validation Set (92%) & Test Set (80%) are also shown below.

<p align="center">
    <img width="850" height="300" src = 'https://github.com/aviralchharia/Brain-Tumor-Segmentation-with-Deep-Neural-Networks/blob/main/Images/Accuracy%20&%20Loss%20Curves.png?raw=true'
</p>
  
<p align="center">
    <img width="400" height="400" src = 'https://github.com/aviralchharia/Brain-Tumor-Segmentation-with-Deep-Neural-Networks/blob/main/Images/Confusion%20Matrix-%20Validation.png?raw=true'
</p>
  
<p align="center">
    <img width="400" height="400" src = 'https://github.com/aviralchharia/Brain-Tumor-Segmentation-with-Deep-Neural-Networks/blob/main/Images/Confusion%20Matrix-%20Test.png?raw=true'
</p>

### Conclusion

We used Convolutional Neural Network to predict whether the subject has Brain Tumor or not from MRI Images. Methods that could be used to increase accuracy includes, using large no. of images i.e., a larger dataset, Hyperparameter Tuning, Using a different Convolutional Neural Network Model may also result in higher accuracy.
