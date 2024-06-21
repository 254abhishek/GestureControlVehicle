# Gesture-Controlled Vehicle with Hand Alignment

This Arduino sketch enables control of a vehicle using hand gestures for directional movements, utilizing an analog sensor to detect hand alignment.

## Table of Contents

- [Overview](#overview)
- [Setup](#setup)
- [Usage](#usage)
- [Components Required](#components-required)
- [Wiring Diagram](#wiring-diagram)
- [Gesture Recognition](#gesture-recognition)
- [License](#license)

## Overview

This project utilizes an Arduino board and an analog sensor to recognize hand gestures for controlling a vehicle's movements:
- **Forward**
- **Backward**
- **Left**
- **Right**
- **Stop**

The vehicle's direction is determined by interpreting hand alignment relative to the analog sensor's position.

## Setup

### Components Required
- Arduino board (e.g., Arduino Uno)
- Analog sensor (e.g., flex sensor, light-dependent resistor, etc.)
- Motor driver module (if using motors)
- DC motors (if applicable)

### Arduino IDE Setup
1. Connect your Arduino board to your computer.
2. Open the Arduino IDE.
3. Copy and paste the provided sketch into a new sketch in the Arduino IDE.
4. Verify and upload the sketch to your Arduino board.

## Usage

1. **Power on your Arduino board and the vehicle setup**.
2. **Gesture Recognition**:
   - Align your hand or fingers with the analog sensor to control the vehicle:
     - **Forward**: Align your hand/fingers in a way that corresponds to moving forward.
     - **Backward**: Align your hand/fingers in a way that corresponds to moving backward.
     - **Left**: Align your hand/fingers in a way that corresponds to turning left.
     - **Right**: Align your hand/fingers in a way that corresponds to turning right.
     - **Stop**: Move your hand/fingers away from the sensor to stop.

3. **Observe** how the vehicle responds to your hand gestures, activating the corresponding motor outputs based on the sensor readings.

## Components Required

- **Arduino Board**: Controls the logic and interprets sensor inputs.
- **Analog Sensor**: Detects hand alignment or gestures.
- **Motor Driver Module**: Translates Arduino's digital signals into motor control signals.
- **DC Motors**: Executes movements based on motor control signals.

## Wiring Diagram

- **Analog Sensor Connections**:
  - Connect the analog sensor to an analog input pin on the Arduino board.

- **Motor Driver Connections**:
  - Connect motor driver outputs (`out1`, `out2`, `out3`, `out4`) to the respective motor terminals.

Ensure proper connections and alignment calibration as per your specific sensor and hardware setup to ensure accurate gesture recognition and vehicle control.

## Gesture Recognition

- The sketch includes logic to interpret analog sensor readings and map them to specific vehicle movements.
- Adjust threshold values or sensor positioning as needed to improve gesture recognition accuracy.

## License

This project is licensed under the [MIT License](LICENSE).
