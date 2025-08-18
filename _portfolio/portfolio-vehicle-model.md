---
title: "Vehicle Modeling in Simulink"
excerpt: "Dynamic vehicle and powertrain modeling in MATLAB/Simulink using real-world parameters of a Mercedes A180.<br/><img src='/images/portfolio/vehicle_model.png'>"
collection: portfolio
date: 2025-02-28
---

## Overview
As part of the *Driver Assistance Systems* course at HTWG Konstanz, I implemented a **vehicle model** in MATLAB/Simulink based on a **Mercedes A180**.  
The goal was to simulate vehicle dynamics under realistic conditions by modeling physical resistances, drivetrain, and driver behavior.  
→ [**Download MATLAB Script (.m)**](/files/portfolio/vehicle_model/vehicle_parameter_Mercedes_A180.m)  
→ [**Download Simulink Model (.slx)**](/files/portfolio/vehicle_model/vehicle_model_cfeng.slx)

The `.m` file provides the **initialization parameters** for the vehicle model and is executed before running the Simulink simulation.

The model was developed step-by-step in five modules:
1. **Vehicle parameters** (mass, aerodynamics, rolling resistance, gear ratios, etc.)
2. **Driving resistances** (air, rolling, gradient resistance)
3. **Dynamic equations** for velocity and distance  
4. **Powertrain model** including engine torque maps and gear losses  
5. **Driver model** with PID control and automatic gear shifting via Stateflow

## Tools & Environment
- **Software:** MATLAB R2024b, Simulink
- **Toolboxes:** Simulink, Stateflow, Control System
- **Modeling techniques:** block-based modeling, interpolation, subsystem abstraction
- **Vehicle reference:** Mercedes A180
