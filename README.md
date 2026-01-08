# ESP32 PID-Based Obstacle Avoidance Robot

## Overview
This project implements a reactive obstacle avoidance robot using an ESP32 and an ultrasonic sensor.
A PID controller dynamically adjusts motor speeds to maintain a safe distance from obstacles.

The system is simulated using Wokwi, enabling hardware-independent testing and validation.


## Features
- Ultrasonic distance sensing (HC-SR04)
- PID-based control for smooth obstacle avoidance
- PWM motor control (simulated using LEDs)
- Real-time serial debugging
- Fully runnable in Wokwi



## System Architecture
Ultrasonic Sensor → PID Controller → Motor Control (PWM)



## Wiring Details

### Ultrasonic Sensor (HC-SR04)

| HC-SR04 Pin | ESP32 GPIO |
|------------|-----------|
| VCC | 5V |
| GND | GND |
| TRIG | GPIO 5 |
| ECHO | GPIO 18 |

### Motor Outputs (Simulation)

Motor behavior is simulated using PWM-controlled LEDs in Wokwi.

| Function | ESP32 GPIO |
|--------|-----------|
| Left Motor | GPIO 26 |
| Right Motor | GPIO 27 |


## Control Logic
- Desired distance (setpoint): **25 cm**
- Distance > 30 cm → Move forward
- Distance between 15–30 cm → PID-based steering
- Distance < 15 cm → Emergency stop



## Components Used
- ESP32
- HC-SR04 Ultrasonic Sensor
- PWM motor outputs (simulated)


