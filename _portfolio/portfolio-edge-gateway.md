---
title: "Edge Gateway for Process Data to IoT Platform"
excerpt: "Containerized edge gateway with MQTT, Node-RED, and ThingsBoard for industrial data transmission and visualization.<br/><img src='/images/portfolio/edge_gateway/edge_gateway.png'>"
collection: portfolio
date: 2025-07-10
---

## Overview
As part of the *Industrial Internet of Things* (IIoT) module in my Master's program in Electrical Systems at HTWG Konstanz, I developed an **edge gateway system** to collect, process, and transmit process data from a production line in the university's automation lab.  
→ [**Download Report (PDF)**](/files/portfolio/edge_gateway/IIoT_EGW_PL_cfeng.pdf)  

The edge gateway gets PLC data via an OPC UA gateway, preprocesses it using **Node-RED**, and forwards it over **MQTT** to the **ThingsBoard IoT platform**. The system enables live visualization, monitoring, and analysis of production and system status data.  
![System Architecture](/images/portfolio/edge_gateway/architecture.png)

## Features
- **Data collection** via MQTT in JSON format
- **Edge processing** using Node-RED and JavaScript mapping
- **Live dashboards** in ThingsBoard for process and system data
- **Containerized architecture** with Docker for modular deployment
- **Monitoring** of gateway health (CPU, RAM, temperature)

## Tech Stack
- **Base Stack:** [IOTstack](https://github.com/SensorsIot/IOTstack) (forked)
- **Edge Tools:** Node-RED, Mosquitto, Docker
- **Cloud Tools:** ThingsBoard, PostgreSQL
- **Hardware:** Linux-based Industrial Edge Gateway ([FR201 OnLogic](https://www.onlogic.com/store/fr201/))
