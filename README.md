# Kaggle-UltrasoundNerveSegmentation

This Kaggle Challenge attempts to find a way to accurately identifying nerve structures in ultrasound images. Data set consists of 5635 ultrasound images and their accompanying mask files, labelling where a collection of nerves called the Brachial Plexus (BP) is. 

For this challenge, I followed jocicmarko's example, using a U-Net convolutional neural network. jocicmarko's work is documented in https://github.com/jocicmarko/ultrasound-nerve-segmentation.  

Since in his original try outs, overfitting manifested, I tried to incorporated image shift, rotation, et al. for data augmentation. No improvement was achieved. 
