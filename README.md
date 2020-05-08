# SocialSafety
Social Distancing Android App with Cough Detection

I really enjoyed working on this project! I'm quite passionate about working on projects which can positively impact lives, and augmenting the social distancing aspect is something that is quite essential to recover from this pandemic. 

The Android App has two activities - 
1. Bluetooth Low Energy based social distance scanning activity. This is meant to run in the background when the user is travelling and can pick up the number of devices that fall within the scanning range of the user's device. It also gets the mac address of those devices to count the number of unique devices the user is interacting with. 

![Bluetooth Based Scanning](link-to-image)

2. Google Maps Location Tracing. This is meant to monitor the user's movements, and makes a note of the places where a user spends more than 15 minutes - while shopping, eating, buying groceries etc. It also plots those locations on a map with a colored marker displaying how crowded that location was by pulling the bluetooth scanning data. The map also plots the road traffic activity to help a user understand if they should go out and travel during this time.

![Crowds on the Map](link-to-image) ![Crowds on the Map](link-to-image)



![Demo Video](link-to-image)


Cough Detection - Used the RandomForrestClassifier as it gave an accuracy of 94%

![Cough Detection](link-to-image)

