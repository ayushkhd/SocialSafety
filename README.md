# SocialSafety
Social Distancing Android App with Cough Detection

I really enjoyed working on this project! I'm quite passionate about working on projects which can positively impact lives, and augmenting the social distancing aspect is something that is quite essential to recover from this pandemic. 

Demo App Video - https://github.com/ayushkhd/SocialSafety/blob/master/Demo.mp4
Cough Demo - 


The Android App has two activities - 
1. Bluetooth Low Energy based social distance scanning activity. This is meant to run in the background when the user is travelling and can pick up the number of devices that fall within the scanning range of the user's device. It also gets the mac address of those devices to count the number of unique devices the user is interacting with. 

![Bluetooth Based Scanning](https://github.com/ayushkhd/SocialSafety/blob/master/Screenshots/Screenshot_20200508-073142_SocialSafety.jpg)

2. Google Maps Location Tracing. This is meant to monitor the user's movements, and makes a note of the places where a user spends more than 15 minutes - while shopping, eating, buying groceries etc. It also plots those locations on a map with a colored marker displaying how crowded that location was by pulling the bluetooth scanning data. The map also plots the road traffic activity to help a user understand if they should go out and travel during this time.

![Crowds on the Map](https://github.com/ayushkhd/SocialSafety/blob/master/Screenshots/Screenshot_20200508-073420_SocialSafety.jpg)

Demo Video - https://github.com/ayushkhd/SocialSafety/blob/master/Demo.mp4

Cough Detection - The RandomForrestClassifier gave us an accuracy of 91%. Used MyActivities app to transmit live data to the classifier which then runs a feature extractor on the raw data using a feature_extractor_manager which calls all the other feature extractor files. The pickle files stored the trained data. The audioclassifier then predicts if there was a cough or other feature using the FluSense Database. The initial plan was to store a count of the 

![MFCC](https://github.com/ayushkhd/SocialSafety/blob/master/Screenshots/Screen%20Shot%202020-05-08%20at%208.48.31%20AM.png)

![power spectral density](https://github.com/ayushkhd/SocialSafety/blob/master/Screenshots/Screen%20Shot%202020-05-08%20at%208.48.27%20AM.png)

![Spectral Flatness(https://github.com/ayushkhd/SocialSafety/blob/master/Screenshots/Screen%20Shot%202020-05-08%20at%208.48.41%20AM.png)

![Overall Feature Importance](https://github.com/ayushkhd/SocialSafety/blob/master/Screenshots/Screen%20Shot%202020-05-08%20at%208.47.51%20AM.png)



Thanks for sharing the dataset! 

https://github.com/Forsad/FluSense-data
@article{10.1145/3381014,
author = {Al Hossain, Forsad and Lover, Andrew A. and Corey, George A. and Reich, Nicholas G. and Rahman, Tauhidur},
title = {FluSense: A Contactless Syndromic Surveillance Platform for Influenza-Like Illness in Hospital Waiting Areas},
year = {2020},
issue_date = {March 2020},
publisher = {Association for Computing Machinery},
url = {https://doi.org/10.1145/3381014},
