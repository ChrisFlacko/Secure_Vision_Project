# Hardware Design Definition
## Hardware
- ESP32-CAM
- AM312 motion sensor
- 5V battery

## Communication
- GPIO (AM312 to ESP32): For triggering capturing photos and wake up ESP32
- WLAN (ESP32 to Host): Send the images to the host

## Software
### Camera_control
This module shall be the main file and contains of the state machine. It controls the program flow and manages to take the photos and trigger the sending.

### Camera_output
This module shall send the pictures via WIFI to the host

### Camera_triger
This module is the connection to the motion sensor and triggers/wakes up the camera

