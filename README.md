# Kaggle-UltrasoundNerveSegmentation

This repository is for an image data augmentation kernel I contributed to the Kaggle Ultrasound Nerve Segmentation challenge. For the specific task of image segmentation, if the image file is shifted, rotated or in any way modified, its accomapnying mask file needs to be modified accordingly. I edited Keras's ImageDataGenerator to realize this function and earned my first Kaggle Kernel bronze medal. 

Besides the image modification methods in Keras's original ImageDataGenerator, I also incorporated elastic transformation based on Bruno G. do Amaral's kernel: https://www.kaggle.com/bguberfain/ultrasound-nerve-segmentation/elastic-transform-for-data-augmentation

The use of this modified ImageDataGenerator is the same as the original Keras ImageDataGenerator, except when creating an ImageDataGenerator object, it accepts extra parameters which are for elastic transformation.

The Kaggle Challenge itself attempts to find a way to accurately identifying nerve structures in ultrasound images. Training data set consists of 5635 ultrasound images and their accompanying mask files, labelling where a collection of nerves called the Brachial Plexus (BP) is. 

For this task, I followed jocicmarko's example, using a U-Net convolutional neural network. jocicmarko's work is documented in https://github.com/jocicmarko/ultrasound-nerve-segmentation. I trained the model and adjusted model parameters, achieving top 29% on the leaderboard. Since my model structure did not differ significantly from his work, my training code is not included here. 


