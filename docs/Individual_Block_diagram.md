---
Rohan Fernandez
EGR 314 - Team 311
---

## Updated Block Diagram for the HMI:
<img src="https://raw.githubusercontent.com/Rohan-Fernandez/Rohan-Fernandez.github.io/refs/heads/main/Images/Individual%20Block%20Diagram%20RF-New%20Final%20block.drawio.png">

## Changes/Updates:
To Coincide with a change in the project's scope, several changes were made to the HMI block diagram, firstly there are only two main buttons now, for sending left and right movement commands to the motor that only take effect when an external mode message is read as being "Manual" (this is sent by the MQTT system). Secondly, the screen was changed to a Songhe OLED screen (provided in class) as there was less data needing to be displayed in the final iteration of the project and also it would work fine as an alternative, especially in reducing the physcial space it takes up. Overall, most of the core ideas present in the block diagram stayed the same, but they were streamlined along with other elements of the project to meet time contraints and ensure that all the systems were able to function together.
