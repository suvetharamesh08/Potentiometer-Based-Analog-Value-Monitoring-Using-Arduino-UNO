#  Potentiometer-Based Analog Value Monitoring Using Arduino UNO

##  Project Overview

This project demonstrates analog value monitoring using an Arduino UNO and a potentiometer. The potentiometer is used to vary the input voltage, which is read through the Arduino's analog input pin (A0). The corresponding analog values are displayed in real time on the Serial Monitor.

This project provides a basic understanding of analog input reading, voltage variation, and sensor interfacing with Arduino.

##  Objectives

- To understand analog input signals using Arduino UNO.
- To interface a potentiometer with an Arduino.
- To monitor changing analog values in real time.
- To understand the working principle of the ADC (Analog-to-Digital Converter).

##  Components Required

- Arduino UNO
- Potentiometer (10kΩ)
- Breadboard
- Jumper Wires
- USB Cable


##  Arduino Code

[View Arduino Code](./potentiometer1.ino)

##  Working Principle

1. The potentiometer generates a variable voltage when its knob is rotated.
2. The variable voltage is supplied to the Arduino's analog pin A0.
3. The Arduino reads the analog voltage using its built-in ADC.
4. The converted digital value is displayed on the Serial Monitor.
5. The readings are updated every 500 milliseconds. 
7. ##  Project Output

![Potentiometer Output](<POTENTIOMETER ..jpeg>)

##  Expected Output

The Arduino UNO reads analog values ranging from **0 to 1023**.

- At minimum rotation: Approximately 0.
- At middle position: Approximately 512.
- At maximum rotation: Approximately 1023.

The readings change according to the position of the potentiometer knob.

##  Applications

- Analog signal monitoring
- Variable voltage measurement
- Sensor interfacing experiments
- Electronic control systems
- Arduino-based embedded projects

