# Smart Water Monitoring System

## Project Overview
**Author:** Deepak K  
**Domain:** Embedded Systems & IoT  
**Date:** September 25, 2026  

The **Smart Water Monitoring System** is an advanced ESP32-based IoT prototype designed for real-time tracking of tank water levels and water flow rates. By integrating dedicated sensors and MQTT cloud messaging, it enables remote water-status tracking, threshold-based monitoring, and automated or manual pump control.

---

## Key Features
* **Real-Time Monitoring:** Continuous tracking of water levels and flow rates using hardware sensors.
* **Cloud Connectivity:** Uses MQTT messaging for seamless and reliable remote telemetry communication.
* **Threshold Alerts & Automation:** Triggers events based on pre-set water thresholds to protect equipment and optimize usage.
* **Remote Pump Control:** Manages pump status remotely or via local automation logic.
* **Wi-Fi Enabled:** Connects directly to local wireless networks for constant cloud synchronization.

---

## Hardware Requirements
* **Microcontroller:** ESP32 development board
* **Sensors:** Ultrasonic water-level sensor & Water-flow sensor
* **Actuators/Outputs:** Relay module and Status LED
* **Power Supply:** Suitable regulated power supply unit

---

## MQTT Topics Configuration
* `water/level_distance_cm` - Publishes current water level / distance measurements.
* `water/flow_rate_lpm` - Publishes water flow rate in liters per minute.
* `water/pump` - Subscribes/Publishes command states for pump operation.

---

## Firmware Details
* **Main Firmware File:** `SmartWaterMonitoring.ino`

---

## Important Notice
Please calibrate the flow sensor and tank-level calculations according to your physical hardware setup before relying on measurements for critical operational decisions.