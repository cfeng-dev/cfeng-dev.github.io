---
title: "STM32 Sensor Interface (GPS & IMU)"
excerpt: "Development of STM32-based drivers and data handling for GPS and IMU in an embedded sensor platform.<br/><img src='/images/portfolio/stm32_gps_imu.png'>"
collection: portfolio
date: 2025-02-10
---

## Overview
As part of the *Embedded Systems* module at HTWG Konstanz, I contributed to a team project in cooperation with [Baumer Group](https://www.baumer.com).  
My task was to develop firmware for **sensor integration and data collection** using the **STM32 NUCLEO-H7A3ZI-Q**.  
→ [**GPS Code Repository**](https://github.com/cfeng-dev/gps_nucleo_h7)  
→ [**IMU Code Repository**](https://github.com/cfeng-dev/imu_bno055_nucleo_h7)  
→ [**KiCad Schematic (.kicad_sch)**](/files/portfolio/stm32/STM32_GPS_IMU.kicad_sch)  

The focus was on integrating a **GPS module (Adafruit Ultimate GPS HAT)** and an **IMU sensor (Adafruit BNO055)**, enabling real-time data processing and transmission for downstream visualization and evaluation.

### BNO055 to STM32 Pin Mapping:

| **BNO055 Pin** | **STM32 H7A3 Pin** |
|----------------|---------------------|
| Vin            | 5V                  |
| GND            | GND                 |
| SDA            | PB9                 |
| SCL            | PB8                 |

### GPS Module to STM32 Pin Mapping:

| **GPS Module Pin** | **STM32 H7A3 Pin** |
|--------------------|--------------------|
| Vin                | 3V3                |
| GND                | GND                |
| RX                 | TX (PB6)           |
| TX                 | RX (PB15)          |
 
### UART Configuration for GPS Module:

| **Parameter**   | **Value**               |
|-----------------|-------------------------|
| Baud Rate       | 9600 Bits/s             |
| Word Length     | 8 Bits (including Parity) |
| Parity          | None                    |
| Stop Bits       | 1                       |

## My Contribution
- Implementation of UART-based communication with **Adafruit Ultimate GPS HAT**  
- I²C-based driver development for **Adafruit BNO055 IMU**  
- **GPS message validation** (NMEA checks, fix state verification)  
- **Real-time data processing** using **FreeRTOS tasks and queues**  
- Formatting and transmission of combined sensor data to a host PC

## Tools & Platform
- **Microcontroller:** STM32 NUCLEO-H7A3ZI-Q  
- **IDE:** STM32CubeIDE  
- **RTOS:** FreeRTOS  
- **Protocols:** UART, I²C, NMEA  
- **Languages:** C
