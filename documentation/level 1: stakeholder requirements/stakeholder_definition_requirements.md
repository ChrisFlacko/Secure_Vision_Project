# Stakeholders
S1: User
S2: Developer
S3: Security Advisor

# Stakeholder needs
S1-N1: The user wants to know who is approaching or standing in front of the door.
S1-N2: The user wants to give the system dataset of persons, to make sure the system is recognizing known persons.
S1-N3: The user wants to be able to add and remove persons, which should be recognized.
S1-N4: The user wants to see the temperature of the room.
S1-N5: The user wants to see the humidity of the room. 
S1-N6: The user wants to see all information on a display.
S1-N7: The user wants to be informed if the temperature exceeds a predefined range.
S1-N8: The user wants to be informed if the humidity exceeds a predefined range.
S1-N9: The user wants the system to be able to run for a long time without shutdown or any charging. 

S2-N1: The developer wants the system to be modular, so that new features can be added easily.

S3-N1: The advisor wants to make sure, that the system is marking a unknown person on the display.
S3-N2: The advisor wants to make sure, that known persons are displayed with their names.
S3-N3: The advisor wants to make sure that the system recognize by itself, if the system is performing in a wrong way.
S3-N4: The advisor needs the system to be secure, so it is secure against any threats from outside. 

# Stakeholder requirements
SH-REQ-1:
The system shall be able to recognize persons within a specific distance.
(S1-N1)

SH-REQ-2:
The system shall classify the persons and compare the faces with the ones in the storage.
(S1-N2)

SH-REQ-3:
The system shall have the ability to add and remove persons from the classification. 
(S1-N3)

SH-REQ-4:
The system shall detect the temperature of the room.
(S1-N4)

SH-REQ-5: 
The system shall display the temperature on a display.
(S1-N4)

SH-REQ-6:
The system shall detect the humidity of the room.
(S1-N5)

SH-REQ-7: 
The system shall display the humidity on a display.
(S1-N5)

SH-REQ-8:
The system shall display the result of the classification of the faces on a display. 
(S1-N6)

SH-REQ-9:
The system shall accept a configurable minimum and maximum temperature threshold. 
(S1-N7)

SH-REQ-10:
The system shall inform the user if the humidity falls outside of the configured min/max humidity range.
(S1-N7)

SH-REQ-11:
The system shall accept a configurable minimum and maximum humidity threshold.
(S1-N8)

SH-REQ-12:
The system shall inform the user if the humidity falls outside of the configured min/max humidity range.
(S1-N8)

SH-REQ-13:
The system shall operate for an extended period without requiring a battery recharge.
(S1-N9)

SH-REQ-14: 
The system shall be build as modular components to add new functionalities easily.
(S2-N1)

SH-REQ-15:
The system shall output an indicator on the display, if a person unknown to the system is detected.
(S3-N1)

SH-REQ-16:
The system shall output the names of the persons on the display, if a person is known to the system.
(S3-N2)

SH-REQ-17:
The system shall have a self-diagnose monitor function to detect, if the program is in a corrupted state.
(S3-N3)

SH-REQ-18:
The system shall reset and restart if a corrupted state is detected.
(S3-N3)

SH-REQ-19:
he system shall minimize its network exposure to threats originating outside the local network.
(S3-N4)