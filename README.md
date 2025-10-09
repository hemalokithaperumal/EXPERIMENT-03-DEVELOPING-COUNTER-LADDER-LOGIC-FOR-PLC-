# EXPERIMENT-03-DEVELOPING-COUNTER-LADDER-LOGIC-FOR-PLC-
## NAME:HEMA LOKITHA P
## REGISTER NUMBER:212223110014
## DEPARTMENT:B.E CSE(IOT)
## YEAR:III

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

<img width="1919" height="1079" alt="Screenshot 2025-10-09 081049" src="https://github.com/user-attachments/assets/6ec10876-577f-40f6-b02d-743ca1137a3f" />

<img width="1919" height="1047" alt="Screenshot 2025-10-09 082010" src="https://github.com/user-attachments/assets/6bd10f2c-a7e9-456e-8b99-0e1e7e810cda" />

<img width="1919" height="1079" alt="Screenshot 2025-10-09 081357" src="https://github.com/user-attachments/assets/131d2a06-bed3-4733-af71-b156c20133be" />

<img width="1919" height="1079" alt="Screenshot 2025-10-09 081447" src="https://github.com/user-attachments/assets/d8aa31ba-0e3c-4692-b424-4144effe7918" />

<img width="1919" height="1079" alt="Screenshot 2025-10-09 081536" src="https://github.com/user-attachments/assets/f6617712-98d6-4987-b0f7-0b9764ec3a36" />

<img width="1919" height="1079" alt="Screenshot 2025-10-09 081551" src="https://github.com/user-attachments/assets/105a22fe-c22a-477c-81cb-336a689e5d66" />

### Results:
The ladder logic programs for Up Counter (CTU), Down Counter (CTD), and Up/Down Counter (CTUD) were successfully implemented and tested. The outputs behaved as expected, indicating correct counting operations. The experiment demonstrated how counters are essential in automation for counting events and managing process sequences.
