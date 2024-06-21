# Arduino Remote Controlled Robot using Joystick and HT12E

This Arduino sketch enables control of a robot using a joystick connected to analog pins and outputs signals through an HT12E encoder IC.

## Table of Contents

- [Overview](#overview)
- [Setup](#setup)
- [Usage](#usage)
- [Joystick Control](#joystick-control)
- [HT12E Output](#ht12e-output)
- [License](#license)

## Overview

This project utilizes an Arduino board to interpret joystick movements from analog pins and encode them using an HT12E encoder IC. The encoded signals control the robot's movements, allowing it to move forward, backward, left, and right based on the joystick's position.

## Setup

### Components Required
- Arduino board (e.g., Arduino Uno)
- Joystick module
- HT12E encoder IC
- Motor driver circuitry and motors

### Wiring Diagram
- **Joystick Connections**:
  - `xPin` (Analog Pin A0) connected to the X-axis output of the joystick.
  - `yPin` (Analog Pin A1) connected to the Y-axis output of the joystick.
- **HT12E Outputs**:
  - `out1` to `out4` connected to the inputs of the HT12E encoder IC.
- **Motor Driver Connections**:
  - Outputs of the HT12E encoder IC connected to the motor driver circuitry controlling the robot's motors.

### Arduino IDE Setup
1. Connect your Arduino board to your computer.
2. Open the Arduino IDE.
3. Copy and paste the provided sketch into a new sketch in the Arduino IDE.
4. Verify and upload the sketch to your Arduino board.

## Usage

1. **Power on your Arduino board and the robot setup**.
2. **Operate the joystick** to control the robot's movements:
   - Move the joystick forward for the robot to move forward.
   - Move the joystick backward for the robot to move backward.
   - Move the joystick left for the robot to turn left.
   - Move the joystick right for the robot to turn right.
   - Release the joystick to stop the robot (`STOP` condition).
   
3. **Observe** the outputs (`out1` to `out4`) changing based on joystick movements, which are then fed into the HT12E encoder IC to control the motors accordingly.

## Joystick Control

- The joystick's X and Y positions are read using analog inputs (`xPin` and `yPin`).
- Based on the joystick's position, the Arduino board determines the direction in which the robot should move.

## HT12E Output

- `out1` to `out4` are digital outputs used to transmit control signals to the HT12E encoder IC.
- These outputs encode directional commands (forward, backward, left, right, stop) from the Arduino based on joystick movements.

## License

This project is licensed under the [MIT License](LICENSE).
