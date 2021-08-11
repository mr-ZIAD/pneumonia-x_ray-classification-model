# pneumonia-x_ray-classification-model
Build a classification model to classify images of chest xrays using Google
AutoML.

for this project i've used Google AutoML, an automated machine learning tool that will allow me to build the model and host it in the cloud.using a dataset from kaggle.com. In order to appreciate how training data impact models, i've build models with 4 variants of the dataset:

1.Create a Clean/Balanced binary classifier
using 100 images from the “normal” class and 100 images from the “pneumonia” class.
2.Create a Clean/Unbalanced binary classifier
use 100 images from the “normal” class, and add 200 more "pneumonia" class images.
3.Create a Dirty/Balanced binary classifier
started with the original dataset of 100 "normal" and 100 "pneumonia" images. Then switches the labels of 30 images in each class.
4.Create a 3-class classifier
using 100 "normal" images, 100 "bacterial pneumonia" images, and 100 "viral pneumonia" images.


