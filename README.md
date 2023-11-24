# Requirements
NumPy version: 1.24.3
SciPy version: 1.7.3
Scikit-learn version: 1.2.2
Pytorch 2.0.0
Tensorflow 2.13.0
---------------------------------------

run the ipynb file as is . just change the dataset path.

The dataset used was "best-artworks-of-all-time" from kaggle.
The dataset contains artists and their painting's images


FIRST PART OF THE CODE IS TRAINED ON DATASET OF ARTIST'S IMAGES.
THE MODEL IS USED FOR CLASSIFICATION OF ARTIST IMAGES
MODEL USED IS RESNET50

REALIZATION HIT AND I REALZED THAT IS NOT THE TASK OF THE ASSIGNMENT 

SO A VGG19 MODEL IS USED TO TRAIN THE IMAGES ON THE STYLE OF A SINGLE ARTIST (VINCENT VAN GOGH IS CHOSEN AS THE DATASET HAD MAX IMAGES OF THE SAID ARTIST)

THE TRAINED MODEL WEIGHTS IS THEN UTILIZED FOR NEURAL STYLE TRANSFER 
ON THE BASE IMAGE USING AN STYLE IMAGE OF THE THE ARTIST 
THE MODEL OUTPUTS A STYLIZED IMAGE 

ALL WEIGHTS OF THE MODEL (BOTH CLASSIFICATION AND THE VGG19STYLE REGRESSION ) AND THE DATASET PATH ARE UPLOADED IN GDRIVE 
https://drive.google.com/drive/folders/1PE0XyglzlwLEJYvCUd-_GFMO-DnBpsH5?usp=sharing

artistdata.rar -----------------> Dataset of artist and their paintings that have been split into train and train dataset in the ratio 90:10
                                  Validation set is taken from train set rseulting in train-valid-test in the ratio 70:20:10
vincentvangogh.rar--------------> Dataset of test and train images of 1 artist ( Vincent Van Gogh )

artistclassify.keras------------> weights of Resnet50 model for classification of the artist given the artist painting images

custom_vgg19_model.pth---------->Vgg19 model pytorch weights that was trained on van gogh paintings only


# Future Improvements
-Train for more epochs and on more better neural network and larger dataset for better training
-Implement different style transfer 
-Deploy a model for specific style or multiple style (depends) and instead of relying on a style image 
  the model can generate a style based on what it was trained on and stylize the image accordingly
