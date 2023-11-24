# Requirements

NumPy version: 1.24.3  
SciPy version: 1.7.3  
Scikit-learn version: 1.2.2
Pytorch 2.0.0  
Tensorflow 2.13.0  

run the ipynb file as is . just change the dataset path.

# Dataset Description

The dataset used was "best-artworks-of-all-time" from kaggle.
The dataset contains artists and their painting's images

# About the ipynb file

The initial segment of the code involves training on a dataset comprising images of various artists, utilizing the ResNet50 model for the classification of these artist images.

Upon reflection, it became evident that this approach was not aligned with the assignment's objectives.

Subsequently, a VGG19 model was employed to train images specifically in the style of a chosen artist, with Vincent van Gogh being selected due to the dataset containing a significant number of his images.

The weights of the trained model are then applied in a neural style transfer process on a base image, using a style image associated with the chosen artist. This process results in the generation of a stylized image.

# Data

All Weights of the model (Both classification and VGG19 style regression) and the dataset have been uploaded in the Gdrive:
https://drive.google.com/drive/folders/1PE0XyglzlwLEJYvCUd-_GFMO-DnBpsH5?usp=sharing
```
artistdata.rar -----------------> Dataset of artist and their paintings that have been split into train and train dataset in the ratio 90:10
                                  Validation set is taken from train set rseulting in train-valid-test in the ratio 70:20:10
vincentvangogh.rar--------------> Dataset of test and train images of 1 artist ( Vincent Van Gogh )

artistclassify.keras------------> weights of Resnet50 model for classification of the artist given the artist painting images

custom_vgg19_model.pth---------->Vgg19 model pytorch weights that was trained on van gogh paintings only
```


# Future Improvements
-Train for more epochs and on more better neural network and larger dataset for better training  
-Implement different style transfer   
-Deploy a model for specific style or multiple style (depends) and instead of relying on a style image   
  the model can generate a style based on what it was trained on and stylize the image accordingly  
-Evaluate the style transfer for with other proper metrics related to style transfer
