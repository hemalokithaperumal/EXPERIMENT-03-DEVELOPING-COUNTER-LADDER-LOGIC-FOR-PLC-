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
<img width="1919" height="1024" alt="Screenshot 2025-10-09 180859" src="https://github.com/user-attachments/assets/00f2c836-5b68-4b28-8b15-41915a0a110d" />
<img width="1919" height="1027" alt="Screenshot 2025-10-09 180920" src="https://github.com/user-attachments/assets/ca7b6916-e75c-4dd6-b967-c0b15f2ba66b" />
<img width="1919" height="1017" alt="Screenshot 2025-10-09 181132" src="https://github.com/user-attachments/assets/b233e776-1698-44a5-8497-111788972995" />
<img width="1919" height="1027" alt="Screenshot 2025-10-09 181159" src="https://github.com/user-attachments/assets/6affbe96-c77c-45a6-bb31-3f5f39a3df99" />
<img width="1917" height="1025" alt="Screenshot 2025-09-25 093220" src="https://github.com/user-attachments/assets/b8d048d2-2a7a-4394-8e8b-6e3357866ab6" />
<img width="1919" height="1029" alt="Screenshot 2025-10-09 181309" src="https://github.com/user-attachments/assets/09cfce8c-b895-436b-8cf7-b31e091c7837" />
<img width="1919" height="1020" alt="Screenshot 2025-10-09 181331" src="https://github.com/user-attachments/assets/a0d24b5b-8c1f-48fb-852c-ca4ccd07a819" />
<img width="1917" height="1016" alt="Screenshot 2025-09-25 093441" src="https://github.com/user-attachments/assets/0a888fef-e842-4614-afaa-536cce284d6f" />


### Results:
The ladder logic programs for Up Counter (CTU), Down Counter (CTD), and Up/Down Counter (CTUD) were successfully implemented and tested. The outputs behaved as expected, indicating correct counting operations. The experiment demonstrated how counters are essential in automation for counting events and managing process sequences.
