
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

# Future Improvements
-Train for more epochs and on more better neural network and larger dataset for better training
-Implement different style transfer 
-Deploy a model for specific style or multiple style (depends) and instead of relying on a style image 
  the model can generate a style based on what it was trained on and stylize the image accordingly
