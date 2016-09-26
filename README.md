# Kaggle-UltrasoundNerveSegmentation

This repository is for an image data augmentation kernel I contributed to the Kaggle Ultrasound Nerve Segmentation challenge. 

This Kaggle Challenge attempts to find a way to accurately identifying nerve structures in ultrasound images. Training data set consists of 5635 ultrasound images and their accompanying mask files, labelling where a collection of nerves called the Brachial Plexus (BP) is. 

For this task, I followed jocicmarko's example, using a U-Net convolutional neural network. jocicmarko's work is documented in https://github.com/jocicmarko/ultrasound-nerve-segmentation. I trained the model and adjusted model parameters, achieving top 29% on the leaderboard. Since I did not improve significantly over his work, my training code is not included here. 

In jocicmarko's original try outs, overfitting manifested, I tried to incorporate image shift, rotation, et al. for data augmentation. For the specific task of image segmentation, if the image file is shifted, rotated or in any way modified, its accomapnying mask file needs to be modified accordingly. I edited Keras's ImageDataGenerator to serve this function and earned my first Kaggle Kernel bronze medal. 
