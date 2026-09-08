# Overview of the project
This project aims to create a secure vision project and smart home. The system shall inform the user about the temperature and humidity of the appartment and also secure the front door by observing it with the camera and inform the user, if a unknown person is there or a known one.

# Learning objectives
The learing objectives includes quiete some topics:
- Low level programming of drivers for sensor and general communication
- High level programming of a neuronal network for classification and detection of faces
- Connection of the high and low level system
- Wifi data communication 

# Scope of the project
The project is split into three systems, a host (Raspberry PI), a sensor client (STM32) and a camera client (ESP32-CAM)
## Host system
- Running the detection algorithmn 
- Running the neuronal network to classify the faces
- Receiving data from the clients
- Display data on the display

## Sensor system
- Receiving data from the host
- Reacting to the host data
- Reading out temperature data
- Reading out humidity data
- Send sensor data to the host
- Security functions to detect corrupt behaviour

## Camera system
- Reading out camera data
- Sending camera data to the host
- Detecting movement in the environment
- Having a energy saving state

# Out of scope 
- Neuronal network from bottom up 