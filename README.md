# Hand Gesture Alexa (Tentative plan, please update with improvements)
A model for detecting eye contact and hand gestures for triggering home automation.

# Goal for Repo
Create a model that can run locally, that can detect direct eye contact, as well as how many fingers the person in the image is holding up, with over 98% accuracy, from between 2 and 15 feet away.

# Architecture
For Gesture recognition, the pipeline I am most familiar with is something like : {FRCNN : human body detection } -> {HRNet : Key point detection -> {Kalman filter : Keypoint Tracker} ->  {STGCN :  Activity detection}
Each of the networks need to be trained independently, but this can be done just by freezing those parts of the network

# Grand Vision
Be able to make eye contact with a camera, and raise a number of fingers at the same time to trigger home automation, like turning off the lights.

# Plan to get data
Photos of multiple hand gestures and eye placement ranging from different races, and face shapes

# Technology stack
