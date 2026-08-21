# Component features
## Linker script
A linker script is necessary to link the different code parts to the designated storage adresses.
- Understand what a linker script needs
- How does it work
- Implement and test of the script

## Startup file
A startup file is necessary cause its the first code which is executed. It puts the vectortable in place, reads out SP and defines interrupt functions.
- Understand the structure and tasks of a startup file
- How it works
- Implement and test of the file

# Bare-Metal-Base
The register definitions are getting imported since there is no educational purpose by writing them on my own. 
Furthermore to mention is, that the code should be structured fully portable.

## HAL
This is the lowest layer and needs to abstract the hardware registers in a portable and modulare way. 

## Drivers
The drivers are implementing the functions for different modules (GPIO, UART etc.). Its using the HAL to make it in an abstract way. The drivers should not directly need/be restricted to the used Chip.

## App
The App is the main code, which is executing the Driver functions to set up everything and later execute the main program.

# Functions

## SysTick
The systick is fundamental to get a time context for the system.

## Timers
Other timers should be implemented to give different funtionalities:
- Modifiable timer
- Delay/wait function

## GPIO
Setting up the GPIO pins needed for the functions

## UART and SPI
Setting up the communication link to the sensor

## PendSV
Already setting up the pendsv for the RTOS which should be implemented later

## CAN
Setting up the CAN for the communication with the host

## Interrupts
Setting up interrupts for:
- Host heartbeat via CAN
- Sensor changes via URAT and SPI

## Bootloader
Setting up a bootloader for secure boot process. 

# Component List
## CAN Communication
This module handles all the CAN communication.

## Sensor manager
This module handles the sensor data by compute and interprete it. 

## Hearthbeat monitor
This module is monitoring the hearthbeat which is getting sent from the host. 

## State machine
This module handles the whole coordination of the different components. 
