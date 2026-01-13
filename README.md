# SensorMaster 10.000

## Overview
SensorMaster 10.000 is a private DIY project created to address a current limitation within the AC Infinity ecosystem:  
the ability to connect and use multiple sensors simultaneously.

The project acts as a Wi-Fi–based multi-sensor hub and automatically detects connected sensor types without manual configuration.

This repository documents the existence, purpose, and capabilities of the project.  
It is **not** a commercial product.

---

## Motivation
AC Infinity offers a growing range of sensors (soil, climate, CO₂, light), but at the time this project was created, only a very limited number of sensors could be connected to a controller at the same time.

During an active grow run, multiple soil sensors were already installed and waiting for an announced sensor hub that had not yet been released.  
To avoid manual swapping of sensors and data gaps, a personal solution was developed.

---

## Supported Sensor Types
Based on the hardware available during development, the following AC Infinity-compatible sensor types are supported:

- Temperature & Humidity sensors  
- CO₂ & Light sensors  
- Soil moisture sensors  

Sensor detection is automatic.

---

## Sensor Data Notes
Some AC Infinity sensors internally provide additional measurement data beyond what is currently exposed by the official controller (e.g. temperature and humidity within the CO₂/light sensor).

This project reads and uses the raw sensor output directly.

Light intensity is exposed both as:
- a calculated **lux value**, based on the underlying sensor characteristics  
- a derived **AI light percentage**, reconstructed by comparison and normalization against controller output behavior  

No proprietary firmware or software from AC Infinity is used.

---

## Home Assistant Integration
Sensor data is published via Wi-Fi and integrated into Home Assistant, allowing centralized monitoring of all connected sensors.

*(Screenshots below)*

---

## Screenshots

![SensorMaster 10.000 Hardware](images/sensormaster.jpg)
![Home Assistant Dashboard](images/homeassistant.png)

---

## Project Scope
- Sensor aggregation only  
- No device control  
- No firmware, schematics, wiring diagrams or source code are provided  

This repository intentionally documents **results**, not build instructions.

---

## Disclaimer
This is a **private, non-commercial DIY project**.

- No affiliation with AC Infinity  
- No products or services are offered  
- No warranties or guarantees  

All product names, trademarks, and brands are the property of their respective owners and are used for identification purposes only.
