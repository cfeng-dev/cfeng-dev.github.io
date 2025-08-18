---
title: "Wind Monitoring System"
excerpt: "Microcontroller software for autonomous wind sensing with Arduino, Modbus, and MQTT.<br/><img src='/images/portfolio/wind_monitoring.png'>"
collection: portfolio
date: 2023-10-26
---

## Overview
As part of a team project at HTWG Konstanz, I developed the **microcontroller software** for a wind monitoring system.  
This embedded system was designed for autonomous deployment at a wind measurement site in Greece and is powered by a solar panel and battery setup.  
→ [**View Code on GitHub**](https://github.com/cfeng-dev/WindTracker_IoT)

The system uses an [Ecowitt WS90 wind sensor](https://www.ecowitt.com/shop/goodsDetail/287) connected via **Modbus (RS-485)** to an **Arduino MKR NB 1500**, with data logging and LTE-based communication.

## My Contribution
- Implemented **RS-485 communication** using the Modbus protocol  
- Logged wind sensor data to **SD card** with timestamp  
- Integrated **FreeRTOS** to manage sensor polling, logging, and communication tasks  
- Used a **watchdog timer** to ensure reliable operation in unattended environments  

## Tools & Hardware
- **Microcontroller:** Arduino MKR NB 1500  
- **Shields:** MKR SD Proto Shield, MKR 485 Shield  
- **Sensor:** Ecowitt WS90  
- **Communication:** Modbus RTU, MQTT over LTE, SMS  
- **Development:** Arduino IDE, C++, SD & NB libraries  
