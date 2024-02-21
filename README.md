## Description
This repository contains a notebook presenting methods to address the challenge of class incremental continual learning (CL) in the context of Human Activity Recognition (HAR). Class incremental continual learning refers to the difficulty faced by models pre-trained on a fixed set of classes when attempting to learn new classes without forgetting the previously learned ones. In this notebook, we explore simple techniques aimed at enabling models to learn from new streams of data while retaining previous knowledge.
The presented two presented and compared methods are *Random replay* and an *iCARL inspired examplar selection*.
The base model, created using **keras**, entails a 1D convolutional network and it processes accelerometer data acquired from subjects performing different activities. Data from both the back accelerometer and the thigh accelerometer are processed simultaneously through separate branches of a convolutional neural network (CNN). Each branch consists of convolutional layers alternated with max pooling layers, whose outputs are concatenated and fed into a dense layer for classification.

This notebook was created for the exam Ambient Intelligence and Domotics at Università degli Studi di Milano Bicocca during november 2023.
## Citations
Employed dataset
Logacjov, Aleksej, Kongsvold, Atle, Bach, Kerstin, Bårdstu, Hilde Bremseth, and Mork, Paul Jarle. (2023). HARTH. UCI Machine Learning Repository. https://doi.org/10.24432/C5NC90.
