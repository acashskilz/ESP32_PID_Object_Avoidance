# ESP32 PID-Based Obstacle Avoidance Robot

## Overview
This project implements a reactive obstacle avoidance robot using an ESP32 and an ultrasonic sensor.
A PID controller adjusts motor speeds to maintain a safe distance from obstacles.

The system is simulated using Wokwi, enabling hardware-independent testing.

## Features
- Ultrasonic distance sensing (HC-SR04)
- PID-based control for smooth obstacle avoidance
- PWM motor control (simulated using LEDs)
- Real-time serial debugging
- Fully runnable in Wokwi

## Control Logic
- Desired distance (setpoint): 25 cm
- If distance is too small, robot turns away
- If distance is too large, robot turns toward the obstacle
- If distance is extremely small, motors stop

## Components Used
- ESP32
- HC-SR04 Ultrasonic Sensor
- PWM Motor Outputs (simulated)

## Notes
This project demonstrates closed-loop control and embedded system design concepts.

