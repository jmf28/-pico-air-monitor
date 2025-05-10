# Pico Air Monitor

A Raspberry Pi Pico project that monitors air quality using a DHT11 temperature/humidity sensor and a potentiometer simulating CO₂ levels. The system displays values on an LCD1602 and uses an LED + buzzer alert if the air quality is poor.

## Features
- 📟 LCD1602 display for live feedback
- 🌡️ DHT11 temperature and humidity sensor
- 🔘 Potentiometer used as analog CO₂ simulator
- 🔔 Buzzer and onboard LED alerts for poor conditions
- 📦 Written in C using the Pico SDK

## Components
- Raspberry Pi Pico
- DHT11 sensor (GPIO 2)
- Potentiometer (connected to ADC pin GPIO 26)
- LCD1602 (I2C – GPIO 0 & 1)
- Buzzer (GPIO 3)
- Onboard LED (GPIO 25)

## Thresholds
- Temperature: 68°F – 78°F optimal
- Humidity: 40% – 55% optimal
- Potentiometer voltage > 2.0V → trigger "High CO₂" alert

## Wiring Diagram
_coming soon (you can add a photo to `/img` folder)_

## Setup
- Install Pico SDK
- Wire components
- Compile with `cmake`
- Flash to Pico via `picotool` or USB drag-and-drop

## License
This project currently has **no license**. Please do not redistribute without permission.

---

👤 Created by Marc Fersan ([Fiverr Profile](https://www.fiverr.com/yourusername))
