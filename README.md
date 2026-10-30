# Grade9-Automatic-Night-Light
# Automatic Lighting System Using Arduino and LDR Sensor

## Project Overview
The Automatic Lighting System is an Arduino-based project that uses a Light Dependent Resistor (LDR) sensor to detect the brightness of the surrounding environment. It automatically turns an LED ON when the environment is dark and OFF when there is enough light.

## Components
- Arduino Uno
- LDR Photoresistor Sensor Module (AO, DO, VCC, GND)
- LED
- 220Ω Resistor
- Jumper Wires

## Input-Process-Output (IPO) System

### INPUT
The LDR sensor detects the surrounding light level and sends an analog signal to Arduino pin A0.

### PROCESS
The Arduino reads the sensor value using `analogRead()` and compares it with a threshold value of 500 using an if-else statement.

- If the light level is below 500, the LED turns ON.
- If the light level is 500 or above, the LED turns OFF.

### OUTPUT
The LED indicates the detected light condition:
- **LED ON** – Dark environment.
- **LED OFF** – Bright environment.

The brightness readings and LED status are also displayed in the Serial Monitor.

## Circuit Connections

LDR VCC	- 5V
LDR GND -	GND
LDR AO -	A0
LED anode (+)	Pin 8 through resistor
LED cathode - (−)	GND
