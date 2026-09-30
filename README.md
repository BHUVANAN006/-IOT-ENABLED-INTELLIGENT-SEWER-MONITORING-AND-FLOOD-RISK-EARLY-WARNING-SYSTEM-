# IoT-Enabled Intelligent Sewer Monitoring and Flood Risk Early-Warning System

## 📌 Project Overview

The **IoT-Enabled Intelligent Sewer Monitoring and Flood Risk Early-Warning System** is an IoT-based monitoring solution designed to continuously monitor sewer and drainage conditions and provide early warnings when abnormal water levels, flow conditions, or rainfall indicate a potential blockage or flood risk.

The system uses sensors connected to an **ESP8266** controller to collect real-time environmental and drainage data. The collected information is processed and displayed through a web dashboard for easy monitoring and early decision-making.

---

## 🎯 Objective

- Monitor sewer and drainage conditions in real time.
- Measure water level and water-flow conditions.
- Detect abnormal conditions that may indicate blockage or overflow.
- Monitor rainfall conditions.
- Identify potential flood-risk situations at an early stage.
- Send real-time data to a web-based monitoring dashboard.
- Provide warning alerts when predefined conditions are detected.

---

## ⚙️ System Architecture

```text
        ┌─────────────────────┐
        │   Sewer / Drainage  │
        └──────────┬──────────┘
                   │
       ┌───────────┼───────────┐
       │           │           │
       ▼           ▼           ▼
  Ultrasonic   Flow Sensor   Rain Sensor
    Sensor
       │           │           │
       └───────────┼───────────┘
                   ▼
            ┌──────────────┐
            │   ESP8266    │
            │ Controller   │
            └──────┬───────┘
                   │
             Wi-Fi Communication
                   │
                   ▼
          ┌───────────────────┐
          │   Web Dashboard   │
          └─────────┬─────────┘
                    │
          ┌─────────┴─────────┐
          ▼                   ▼
    Live Monitoring       Risk Alerts
