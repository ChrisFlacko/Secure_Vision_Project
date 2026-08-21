# Container overview
## Hardware
The following hardware is used to realize the system:
- Host: Raspberry pi
- Client: STM32F303RE (Cortex M4)
- Camera: USB camera
- Temperature sensor: tbh
- Humidity sensor: tbh

## Software
The following software approaches are made:
- Host: Python to perform the high level camera operations
- Client: C for low level programming of a bare metal program and later RTOS and control functions

## Communication
The following communication protocols are used:
- Host <-> Client: CAN (later maybe Ethernet)
- Host <-> Camera: USB
- Client <-> Sensor: UART 