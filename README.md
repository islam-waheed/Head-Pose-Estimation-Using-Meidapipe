# Head-Pose-Estimation-Using-Meidapipe

Head Pose Estimation
In this project we will draw the 3 position axis (pitch,yaw,roll) by predicting the 3 angels of each position by training 3 models to predict each angel.
We will use AFLW2000 dataset with contains 2000 image and 2000 matlab file with contains the 3 labels (angels).
We will use MediaPipe library in both training and testing phases:
In Training: first we dtect the face of each image then using the same library to generate the landmark points of the face after this phase the training data (features) will contain 1853 samples with 936 columns (468 for X and 468 for Y), for labels we will extract the 3 angels from the mat file.
In Testing: we will use the MediaPipe Library to generate the landmarks as we did in the training phase and using the trained models to predict the 3 labels and using them to draw the axis.

HeadPoseResult.gif
