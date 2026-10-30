Potentiometer-Based Analog Value Monitoring Using Arduino UNO
📌 Project Overview

This project demonstrates the interfacing of a Potentiometer with an Arduino UNO to read and monitor variable analog voltage values.

A potentiometer acts as a variable resistor that allows users to adjust the output voltage by rotating its knob. The Arduino reads the changing analog voltage through its analog input pin (A0) using the analogRead() function.

The corresponding analog values are displayed in real time through the Serial Monitor.

This project helps understand analog input processing, voltage variation, and sensor interfacing with Arduino.

🎯 Project Objectives
Understand the working principle of a potentiometer.
Interface a potentiometer with Arduino UNO.
Read variable analog values using the A0 pin.
Understand analog-to-digital conversion (ADC).
Display real-time analog readings using Serial Communication.
🛠️ Components Required
S.No	Component	Quantity
1	Arduino UNO	1
2	Potentiometer (10KΩ recommended)	1
3	Breadboard	1
4	Jumper Wires	As required
5	USB Data Cable	1
⚙️ Working Principle

A potentiometer consists of three terminals and works as a variable voltage divider.

When the knob is rotated, the output voltage changes accordingly.

Minimum Position: Analog reading approaches 0.
Middle Position: Analog reading is approximately 512.
Maximum Position: Analog reading approaches 1023.

The Arduino UNO converts the analog voltage into a digital value using its 10-bit ADC and displays the result on the Serial Monitor.

🔌 Pin Configuration
Potentiometer Pin	Arduino UNO
First Terminal	5V
Middle Terminal (Output)	A0
Third Terminal	GND
💻 Arduino Code
void setup() {
  Serial.begin(9600);
}

void loop() {
  int value = analogRead(A0);

  Serial.print(value);

  delay(500);
}
📊 Expected Output

The Serial Monitor displays changing analog values depending on the potentiometer knob position.

Example:

0
125
256
512
768
900
1023
