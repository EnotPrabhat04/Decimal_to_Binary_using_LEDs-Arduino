Arduino Binary to Decimal Converter

Overview

This project demonstrates how to represent a decimal number (from 0 to 15) as a 4-bit binary output using an Arduino. It uses four LEDs connected to GPIO pins to display the binary equivalent of the given decimal number. The user inputs a number through the Serial Monitor, and the corresponding binary representation is shown on the LEDs.

**Features**

1.Converts decimal numbers (0-15) to their binary representation

2.Displays the binary output using four LEDs

3.Simple serial communication for input

4.Error handling for invalid inputs

**Components Used**

Arduino Board,4 LEDs,4 Resistors (220Ω each),

**Connecting Wires**

USB Cable for Programming

**Circuit Connections**

Pin 8 -> LED 1 (LSB)

Pin 9 -> LED 2

Pin 10 -> LED 3

Pin 11 -> LED 4 (MSB)

Connect the other side of each LED to GND through a 220Ω resistor.

**Working Principle**

The user enters a number between 0 and 15 using the Serial Monitor.

The Arduino reads the input using Serial.parseInt().

Using a switch statement, it controls the LEDs by writing HIGH or LOW to the corresponding pins.

If the input is outside the 0-15 range, an error message is displayed.

**Code Explanation**

**1.Pin Initialization:** int pin1 = 8, pin2 = 9, pin3 = 10, pin4 = 11;

**2.Serial Communication:** Serial.begin(9600);

**3.Switch Case for Binary Representation:**

Based on the input, the LEDs are controlled using digitalWrite() statements.

**4.Error Handling:**
If the user enters a number outside the valid range, it prints an error message using Serial.println().

**Conclusion**

This project provides a simple yet effective way to demonstrate how binary numbers are represented and visualized using LEDs. It's a great educational tool for beginners to understand number systems and Arduino programming.
