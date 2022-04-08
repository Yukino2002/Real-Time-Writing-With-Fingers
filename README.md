# Real-Time-Writing-With-Fingers

## Introduction

The application allows users to `write on their videos using their fingers in real-time`. It can be used for quick explanations during meetings or maybe online classes. The input feed is taken through the webcam which is parsed through a python script.

Using the `mediapipe` package provided by Google, the user's hand is detected and segmented into 21 landmark points. The coordinates obtained are in turn used to accurately locate,
draw, erase etc depending on the gesture made using the `OpenCV` module available. The user can change the color as well the sizes of the brush and the eraser.

The gestures as follows:

1. `Index finger:` Used to draw on the video.

2. `Index + middle finger:` Used to move around the video and navigate through the navigation bar.

3. `Index + middle + ring + little finger:` Used to erase the written text. 

## Methodology

1. `Processing the video:` This is done through the webcam and it
is accessed using the OpenCV module available in python.
The video had to be inverted as the default is not
laterally inverted.

2. Creating the gesture recognition object: Using the
mediapipe module provided by Google, we create a class
object capable of detecting the user’s hand and return the
list of 21 landmark points. By manipulating the
coordinates, we can specify the gesture and hence assign
functionalities accordingly.

3. Drawing on the video feed: Using the coordinates, we can
accurately draw through the OpenCV module. The thickness of
the brush, eraser etc. can be adjusted.