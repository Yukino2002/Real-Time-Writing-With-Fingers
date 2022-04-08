# Real-Time-Writing-With-Fingers

## Introduction

The application allows users to `write on their videos using their fingers in real-time`. It can be used for quick explanations during meetings or maybe online classes. The input feed is taken through the webcam which is parsed through a python script.

Using the `mediapipe` package provided by Google, the user's hand is detected and segmented into 21 landmark points. The coordinates obtained are in turn used to accurately locate,
draw, erase etc depending on the gesture made using the `OpenCV` module available. The user can change the color as well the sizes of the brush and the eraser.

## Methodology

