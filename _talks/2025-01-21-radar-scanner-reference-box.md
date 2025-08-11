---
title: "Embedded Systems – Radar Scanner Reference Box"
collection: talks
type: "Project Presentation"
permalink: /talks/2025-01-21-radar-scanner-reference-box
venue: "HTWG Konstanz, Department of Electrical Engineering and Information Technology"
date: 2025-01-21
location: "Konstanz, Germany"
---

Project presentation as part of the *Embedded Systems* module on the development of a radar scanner reference box.  

The project, conducted in cooperation between [HTWG Konstanz](https://www.htwg-konstanz.de) and [Baumer Group](https://www.baumer.com), covered hardware design, firmware development, sensor integration ([Adafruit Ultimate GPS HAT](https://www.adafruit.com/product/2324), [Adafruit BNO055 IMU](https://www.adafruit.com/product/2472), [STM32 NUCLEO-H7A3ZI-Q](https://www.st.com/en/evaluation-tools/nucleo-h7a3zi-q.html), camera), data fusion, and visualization.  

My responsibility in the project was **software development for sensor data collection**, including IMU data processing, GPS data processing, GPS data verification, and combined IMU and GPS data collection. This involved implementing real-time data synchronization via FreeRTOS tasks, validating GPS messages, transmitting data to the PC, and integrating the data streams for further processing and visualization.  

📄 [Download presentation]({{ "/files/presentations/ES_BRT.pdf" | relative_url }})
