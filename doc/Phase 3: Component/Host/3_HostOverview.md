# Overview
The host system is build inside a linux environment. Therefore a devconatiner is not needed and only a virtual environment is created. 

# Component features
## Can
Provides the CAN socket 

## Camera
Provides the camera interface via openCV

## Supervisior
Combines the camera and can to decide what to do.
### Face detection
This subtask detects faces
### Face recognition
This subtask is recognizing the detected faces
### Face database
This holds all the known faces
### Action handler
This subtask is executing the corresponding action.

## Health
Send heartbeat and evaluate health status
