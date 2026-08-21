# Base structure
## Fundamental
### Container
For the reproducable environment a devcontainer is set up using docker. There the build process is defined by the programs and their individual version which is used.

### CI/CD
The CI/CD test pipeline is implemented on github, using also the same docker image. 

### CMake
For compiling the code, cmake is used. The section is finished, when:
- CMake structure is understood
- How does the compiling work
- Implementation and testing of the CMake features

### Unit Tests
Each function must be written in a modular way, that unit tests can be written for them. 

### CAN definitions
A submodul must be create for the shared information between the host and the client, a so called submodule. There are for example the definitions of the CAN messages and different enums on how to interprete data which is used on both components.

# Component responibilities  
## Host PI
The host needs a program, which is able to read in camera data, compute the data and interprete it. 

The host needs to have a neuronal net in order to interprete if the camera is detecting a human face.

The host needs to have a database of known faces.

The host needs to be able to recognize known faces.

The host needs to be able to take action if it recognizes a face. 

The host needs to send a heartbeat over CAN (or Ethernet). 

The host needs to be able to receive sensor data. 

The host needs handlers to react to the sensor data.

## Client STM32
The client needs to have a deterministic state machine or a RTOS.

The client needs to be able to receive messages over CAN (later Ethernet).

The client needs to be able to send messages over CAN (Later Ethernet).

The client needs to have communication to sensors. 

The client needs to check the heartbeat of the host. 

The client needs to implement a small neuronal network. 


