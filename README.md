##Hand Gesture Recognition Using FRDM KL25Z Board
This project implements hand gesture recognition using the FRDM KL25Z development board, which includes a Cortex-M0+ processor and an inbuilt accelerometer. The project uses the Keil uVision IDE for programming the board in ARM assembly or C. Hand movements along the X, Y, and Z axes are detected by the board's accelerometer, and specific gestures are recognized by monitoring changes in the accelerometer's output. These gestures are then used to control external devices through output ports.

##Project Aim
The goal of this project is to recognize hand gestures and use them to control external devices through output ports. An oscilloscope is used to visualize the changes in accelerometer values as voltage waveforms, which vary in response to hand movements.

##Components Required
FRDM KL25Z board (with Cortex-M0+ processor)
Oscilloscope
Oscilloscope probes
Wires
Software Used
Keil uVision IDE: An integrated development environment (IDE) for developing embedded software on ARM-based microcontrollers.
##Project Overview
The project involves the following steps:

1)Board Setup: The FRDM KL25Z board's inbuilt accelerometer is accessed via the I2C port.<br>
2)Gesture Detection: As the board is moved along the X, Y, and Z directions, the accelerometer captures these movements, recording their values.<br>
3)Thresholding: The recorded accelerometer values are compared against predefined thresholds to recognize specific hand gestures.<br>
4)LED Control: The internal LEDs of the board are programmed to light up in different colors (Red, Blue, Green) based on the movement direction (X, Y, Z).<br>
5)Oscilloscope Output: The output ports of the board are connected to an oscilloscope instead of external LEDs. The X and Y accelerometer values control the waveforms displayed on the oscilloscope, causing them to stretch or shrink (i.e., increase or decrease).<br>
6)Gesture-Based Device Control: Using the changes in the accelerometer values, external devices can be controlled through hand gestures.<br>
##Procedure
Program the FRDM KL25Z Board: Write code in ARM assembly or C using Keil uVision to interact with the accelerometer and output ports.<br>
Accelerometer Access: Use the I2C interface to obtain accelerometer readings.<br>
Gesture Recognition: Implement code to check for specific thresholds in accelerometer values that correspond to hand gestures.<br>
LED and Oscilloscope Control: Use the accelerometer values to control the board's internal LEDs and oscilloscope output.<br>
