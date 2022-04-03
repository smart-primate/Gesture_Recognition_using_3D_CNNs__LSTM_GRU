GESTURE RECOGNITION TO CONTROL TV - PROBLEM STATEMENT

The objective of this project is to develop a cool feature in the smart TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.

The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:
 - Thumbs up:  Increase the volume
 - Thumbs down: Decrease the volume
 - Left swipe: 'Jump' backwards 10 seconds
 - Right swipe: 'Jump' forward 10 seconds  
 - Stop: Pause the movie
 
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use. 

All images in a particular video subfolder have the same dimensions but different videos may have different dimensions. Specifically, videos have two types of dimensions - either 360x360 or 120x160 (depending on the webcam used to record the videos). Hence, some pre-processing is required to standardise the videos. 

Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.

In this project, I have tried to build the model using both 3D CNNs as well as RNN-based structures like LSTM and GRU. A comparison has been performed between the two arhitectures over several models to obtain the most reliable predictions for the gestures.

The training and validation data can be found @ https://drive.google.com/drive/folders/1QJ5RHBr22ovdHNDENtDpWg59OxsjzrOY?usp=sharing
