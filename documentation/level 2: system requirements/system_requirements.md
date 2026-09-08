# System requirements
SYS-REQ-1:
The system shall detect the presense of a person in front of the door.
(SH-REQ-1)

SYS-REQ-2:
The system shall detect persons within a range of 4 meters. 
(SH-REQ-1)

SYS-REQ-3:
The system shall classify persons within a range of 2 meters. 
(SH-REQ-2)

SYS-REQ-4:
The system shall classify persons by comparing the face to the stored data. 
(SH-REQ-2)

SYS-REQ-5:
When a person is detected within range, the system shall complete classification within 5 seconds.
(SH-REQ-2)

SYS-REQ-6:
The system shall determine, for each classified face, whether it matches a known person or is unknown.
(SH-REQ-2)

SYS-REQ-7:
The system shall store facial data of known persons for comparison purposes.
(SH-REQ-2)(SH-REQ-3)

SYS-REQ-8:
The system shall be able to remove the facial data of a person and their name.
(SH-REQ-3)

SYS-REQ-31:
The system shall be able to add the facial data of a person and their name.
(SH-REQ-3)

SYS-REQ-9:
The system shall measure the room temperature within a range of 10°C to 40°C with an accuracy of ±0.5°C.
(SH-REQ-4)

SYS-REQ-10:
The system shall update the room temperature every 30 seconds.
(SH-REQ-4)

SYS-REQ-11:
The system shall show the temperature in celcius on the display.
(SH-REQ-5)

SYS-REQ-12:
The system shall measure the room humidity within a range of 10% to 100% with an accuracy of ±0.5%.
(SH-REQ-6)

SYS-REQ-13:
The system shall update the room humidity every 30 seconds.
(SH-REQ-6)

SYS-REQ-14:
The system shall show the humidity in percentage on the display.
(SH-REQ-7)

SYS-REQ-15:
The system shall show the detected face on the display. 
(SH-REQ-8)

SYS-REQ-16:
The system shall give information on the display, if the face is known or not by the system.
(SH-REQ-15)

SYS-REQ-25:
The system shall output the name of the person on the display, if the person is known. 
(SH-REQ-16)

SYS-REQ-17:
The system shall accept a minumum and maximum value for the temperature.
(SH-REQ-9)

SYS-REQ-18:
The system shall inform the user over the display, if the temperature is falling out of the min/max temperature range.
(SH-REQ-10)

SYS-REQ-19:
The system shall have a default min/max temperature preconfigured.
(SH-REQ-10)

SYS-REQ-20:
The system shall accept a minumum and maximum value for the humidity.
(SH-REQ-11)

SYS-REQ-21:
The system shall inform the user over the display, if the humidity is falling out of the min/max humidity range.
(SH-REQ-12)

SYS-REQ-22:
The system shall have a default min/max humidity preconfigured.
(SH-REQ-12)

SYS-REQ-23:
The system shall only operate to take sensor measurements and display them. Otherwise it shall be in a power saving state. That means it shall consume less than 10mA.
(SH-REQ-13)

SYS-REQ-24:
The system shall have for every function it's own component, so it can be activated and deactivated without interfere the general program.
(SH-REQ-14)

SYS-REQ-26:
The system shall check the program flow every 1 second after SYS-REQ-27/28.
(SH-REQ-17)

SYS-REQ-27:
The system shall check the temperature data if it is plausible or not. If the temperature for 2 measurements is over 2 degrees, the temperature value shall be filtered instead of using the measured one (high indication of corruption).
(SH-REQ-17)

SYS-REQ-28:
The system shall check the humidity data if it is plausible or not. If the humidity for 2 measurements is over 5 percent, the humidity value shall be filtered instead of using the measured one (high indication of corruption).
(SH-REQ-17)

SYS-REQ-29:
The system shall trigger a reset, if a corrupted state is detected.
(SH-REQ-18)

SYS-REQ-30:
The system shall operate within a local network with no direct connection to external networks.
(SH-REQ-19)