# classification model to classify chest x-ray images using Google AutoML.

for this project i've used Google AutoML, an automated machine learning tool that allowes me to build the model and host it in the cloud using a dataset from kaggle.com. In order to appreciate how training data impact models, i've build models with 4 variants of the dataset:

1.Clean/Balanced binary classifier
<img width="948" alt="Clean:Balanced" src="https://user-images.githubusercontent.com/87137785/129297660-768268b9-328c-4893-a96f-1c72de53fccf.png">

using 100 images from the “normal” class and 100 images from the “pneumonia” class.

2.Clean/Unbalanced binary classifier

<img width="965" alt="Clean:Unbalanced" src="https://user-images.githubusercontent.com/87137785/129297696-200b8993-7b8e-4e29-a3d7-5a9b8c3da3ed.png">

using 100 images from the “normal” class, and add 200 more "pneumonia" class images.

with unbalanced data the model learn significantly more about pneumonia class than normal class.


3.Dirty/Balanced binary classifier

<img width="948" alt="Dirty:Balanced" src="https://user-images.githubusercontent.com/87137785/129297717-569fc4a7-8ebd-4467-a4f4-9aad06921a4f.png">

started with the original dataset of 100 "normal" and 100 "pneumonia" images. Then switches the labels of 30 images in each class.

Dirty data confuse the model as we can see that 86% of the true pneumonia were classified 14% of the time in the normal category.

4.3-class classifier

<img width="955" alt="3-class" src="https://user-images.githubusercontent.com/87137785/129297735-e18b3ffb-548d-4772-83ba-5dfc48def8e6.png">

using 100 "normal" images, 100 "bacterial pneumonia" images, and 100 "viral pneumonia" images.

viral pneumonia class is most likely to confuse the model.


