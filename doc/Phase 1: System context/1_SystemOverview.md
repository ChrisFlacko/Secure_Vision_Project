# Project Overview
## General description
This project is designed to plan and execute a project with a real life application. Therefore the system needs to be described, as well as its functionality and the corresponding components, which are needed for the execution. 

## Project goal
The goal is to design a system, which is able to read out camera data on a "host" system and handle this data. In addition to the host there is a client which is real-time system and communicates with the host and is controlled by him. The client does also have its own sensors to monitor the temperature and other diagnostic features.

## General requirements
### Host system
The host system needs to be a high power device, which needs to be able to handle and compute camera data. It also needs to have certain communication links in order to communicate with the client, surrounding and also be able to connect to the internet. 

### Client system
The client does not need so much power, but needs low level determenistic behaviour instead to be able to run a real time operating system and control the host. But in the beginning a bare metal program should be sufficient.  
The client needs to check the heartbeat and has a State machine which is reactive to the messages from the host.

## Timeline
The following steps are defined in order to achieve the goal:
1. Define the system context and draft architecture via the C4-Model (Phase 1–3)
2. Derive functional and non-functional requirements; validate the C4 draft against them and revise where they conflict
3. Define component interfaces (Host <-> Client message format, internal component contracts)
4. Implement the environment:
   4.1. Docker image
   4.2. CMake for VS Code
   4.3. Project structure for host and client
   4.4. CI/CD pipeline
   4.5. Linker script and startup script (see Client/3_ClientOverview.md)
   4.6. Initial push
5. Verify implementation against acceptance criteria
