# ESP32 Smart Machine Health Monitor

## Overview
This project is an industrial machine health monitoring system using ESP32 and MPU6050.

It monitors vibration levels from the MPU6050 accelerometer and classifies machine condition into NORMAL, WARNING, and CRITICAL states. A buzzer alert is triggered when abnormal vibration is detected.

## Features
- Real-time vibration monitoring
- MPU6050 accelerometer interfacing using I2C
- Machine health classification
- Buzzer-based alert system
- ESP32-based embedded firmware
- Industrial IoT and predictive maintenance concept

## Hardware Used
- ESP32 Development Board
- MPU6050 Accelerometer and Gyroscope Sensor
- Buzzer
- Jumper Wires
- Breadboard

## Pin Connections

| Component | ESP32 Pin |
|---|---|
| MPU6050 SDA | GPIO21 |
| MPU6050 SCL | GPIO22 |
| MPU6050 VCC | 3.3V |
| MPU6050 GND | GND |
| Buzzer Positive | GPIO25 |
| Buzzer Negative | GND |

## Working Logic

The ESP32 reads acceleration values from MPU6050 through I2C communication.

A vibration value is calculated from X, Y and Z acceleration data.

Based on the vibration value, the system classifies machine condition:

| Condition | Vibration Level |
|---|---|
| NORMAL | Low vibration |
| WARNING | Medium vibration |
| CRITICAL | High vibration |

## Software Stack
- Embedded C / Arduino C++
- Arduino IDE
- ESP32 Arduino Core
- I2C Communication
- Sensor Data Processing

## Future Improvements
- MQTT cloud dashboard
- ThingsBoard integration
- FreeRTOS task separation
- Data logging
- Relay-based machine cutoff
- Mobile alert system

## Project Status
Planning and hardware setup stage. Breadboard-based hardware implementation will be completed next.
