# EXPERIMENT-03-DEVELOPING-COUNTER-LADDER-LOGIC-FOR-PLC-
## NAME: HEMA LOKITHA P
## REGISTER NUMBER: 212223110014
## DEPARTMENT: B.E CSE-IOT
## YEAR: III

### Aim:
To understand and implement various counter operations in Programmable Logic Controller (PLC) ladder logic.

### Apparatus Required:
Programmable Logic Controller (PLC): A PLC that supports counter functions.
PLC Programming Software: Software such as RSLogix, TIA Portal, or CX-Programmer.
Computer System: For programming and simulating the PLC ladder logic.
Input Devices: Push buttons or switches to trigger the counter operations.
Output Devices: LEDs or other indicators to visualize the counter outputs.
Wires and Connectors: For interfacing input/output devices with the PLC.
Power Supply: Appropriate power supply for the PLC and peripherals.

### Theory:
Counters in PLCs are used to count events or occurrences, such as the number of items passing on a conveyor belt, the number of cycles a machine runs, or how many times a process has started or stopped. Counters are commonly used in automation to perform tasks like stopping a machine after a set number of products or signaling a notification when a count reaches a specific value.

### Types of Counters:
Up Counter (CTU) Functionality:

The up counter counts every time the input condition becomes TRUE (ON). When the accumulated value reaches the preset value, the counter output becomes TRUE. If the reset input is triggered, the counter resets to zero.
Down Counter (CTD) Functionality:

The down counter decreases the count every time the input condition becomes TRUE (ON). When the count reaches zero, the counter output becomes TRUE. The counter can be reset by a reset input to the preset value.
Up/Down Counter (CTUD) Functionality:

The up/down counter can increment or decrement the count based on two different inputs. One input increments the count, while the other decrements it. When the count reaches the preset value or zero, the respective outputs become TRUE. The counter can be reset as required.


### Procedure:
Setup the PLC Programming Environment:
Connect the PLC to the computer and launch the PLC programming software.
Ensure all input and output devices are connected to the PLC’s I/O modules.
Create Ladder Logic for Counters:
Up Counter (CTU):

Create a rung with an input (e.g., a push button) linked to a CTU instruction.
Set the preset value (e.g., 10 counts). Assign an output to indicate when the preset value is reached.
Down Counter (CTD):

Create a rung with an input linked to a CTD instruction.
Set the preset value (e.g., 5 counts). Assign an output to indicate when the counter reaches zero.
Up/Down Counter (CTUD):

Create a rung with separate inputs for counting up and counting down.
Set the preset value (e.g., 8 counts). Assign outputs for when the count reaches the preset value or zero.
Simulate the Ladder Logic:
Up Counter (CTU):

Run the simulation in the PLC software. Press the input button repeatedly and observe the counter increment until the preset value is reached, at which point the output activates.
Down Counter (CTD):

Run the simulation, press the input button repeatedly, and observe the counter decrement. When the counter reaches zero, the output activates.
Up/Down Counter (CTUD):

Simulate both the up and down counting inputs. Observe how the counter increments or decrements and how the output is activated when the count reaches the preset value or zero.
Download and Execute:
Download the ladder logic program to the PLC if available and run it.
Test the counters with the physical push buttons and observe the LEDs or other output devices.
### Outputs:
Up Counter (CTU): The output LED or indicator should activate when the preset count (e.g., 10) is reached.
Down Counter (CTD): The output should activate when the count reaches zero.
Up/Down Counter (CTUD): The output should activate when the count reaches the preset value or zero, depending on the inputs.

### Simulation Screenshots:

## COUNTER
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/3d792162-c3b1-4d7b-aea1-05f909f81393" />

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/588ed7cd-a508-4c4c-a655-96773766ba72" />

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/bed34e51-b255-4f28-8516-d1fc82b982fe" />

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/8ee0f09a-cddf-42fd-b5fe-a84979436f33" />

<img width="1907" height="1018" alt="image" src="https://github.com/user-attachments/assets/1139d689-53b0-42cb-b9d7-8710a15b1624" />

<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/adfad714-e0a3-4c13-a8a6-6bf65e28a857" />


## UP COUNTER

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/8d7cb89b-ea79-4418-b2c1-c55954c6da89" />

<img width="1500" height="250" alt="image" src="https://github.com/user-attachments/assets/4e36844f-8339-4955-a8ac-546ac911c502" />

## DOWN COUNTER:

<img width="1463" height="647" alt="image" src="https://github.com/user-attachments/assets/2ef0e879-0d42-49af-81aa-2f81f6bfbffd" />

<img width="1351" height="375" alt="image" src="https://github.com/user-attachments/assets/6fbc8194-a41c-4cbb-82e6-4f4c3c139f63" />

<img width="1504" height="339" alt="image" src="https://github.com/user-attachments/assets/d6d9303e-a63d-4457-a407-f3159c220e11" />

<img width="1504" height="339" alt="image" src="https://github.com/user-attachments/assets/a84c6fbc-33cb-4a33-87e1-2c216595bf66" />

<img width="1509" height="312" alt="image" src="https://github.com/user-attachments/assets/692a7ec8-21c6-4ef9-9f02-cfd1f190732c" />

## UP/DOWN COUNTER

<img width="1606" height="651" alt="image" src="https://github.com/user-attachments/assets/d709a71e-1f57-421b-921d-d08d443d4084" />

<img width="1406" height="548" alt="image" src="https://github.com/user-attachments/assets/50413fbe-d037-4f90-9aac-f70efefd1830" />

<img width="1505" height="220" alt="image" src="https://github.com/user-attachments/assets/1b52c3a6-1ea9-4968-87da-4373b857fc5e" />

<img width="1503" height="193" alt="image" src="https://github.com/user-attachments/assets/7005b4cd-5008-424c-9d93-f4f19ca5704c" />

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/7e9577e4-117e-4725-b834-5148c71aef5e" />

### Results:
The ladder logic programs for Up Counter (CTU), Down Counter (CTD), and Up/Down Counter (CTUD) were successfully implemented and tested. The outputs behaved as expected, indicating correct counting operations. The experiment demonstrated how counters are essential in automation for counting events and managing process sequences.
