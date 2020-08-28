# DL--Project_Series_10---Image_Retrieval_System_using_Autoencoder

## Project Name: Image Retrieval using Autoencoder and K Nearest Neighbors

### Aim: 


The program should accept an image and return N number of images similar to the user provided image from the dataset using auto encoder and k nearest neighbor technique.


### Methodology:


The dataset consisted of 4728 images of various animals such as Tiger, Lion, Cheetah, Fox etc. For our task, auto encoder network was used, which compresses the input image into a latent-space representation (using encoder network), and then reconstruct the output image from this representation (using decoder network). This latent representation was successful in learning to compress the visual image into latent representation, this means that all the similar images will encoded in similar way by using the encoder network (this concept was used for image retrieval task).

The first step is to train the auto encoder with the training set, for making the encoder to learn how to compress the image to latent representation. After training, only encoder part is used for further analysis. The same encoding has to be done in searching database too, where we want to find the similar images for the user prescribed image (this too needed to encode). We then compare the input image with the database and find the comparison using K nearest neighbor technique. By this similar image can be extracted from the searching database.

