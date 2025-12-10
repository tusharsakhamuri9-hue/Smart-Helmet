# Smart Helmet Safety System

A safety-focused helmet integrating accident detection and live tracking. It identifies accident conditions or helmet removal using sensors and automatically sends an SMS alert with GPS coordinates to an emergency contact using a GSM module.

---

## Table of Contents
1. Overview
2. Features
3. Hardware Requirements
4. System Architecture
5. Circuit Connection Guide
6. Working Principle
7. Arduino Code
8. SMS Alert Format
9. Future Enhancements
10. Project Images
11. License

---

## 1. Overview

Road safety is one of the most critical concerns for two-wheeler riders. The Smart Helmet Safety System enhances safety by ensuring that if an accident occurs, the system will immediately notify emergency contacts with real-time location details, enabling faster rescue response.

This solution uses GSM + GPS modules along with sensors installed inside the helmet.

---

## 2. Features

- Helmet tilt detection using analog tilt sensor
- Accident impact detection via limit switch
- Live GPS location alert with latitude & longitude
- Automatic SMS alert to emergency contacts using SIM900
- LED safety indicator during emergency alert
- Low-cost and easy to implement

---

## 3. Hardware Requirements

| Component | Description |
|----------|-------------|
| Arduino Uno / Nano | Microcontroller |
| NEO-6M GPS Module | Coordinates tracking |
| SIM900 GSM Module | SMS alert communication |
| Tilt Sensor | Helmet tilt / fall detection |
| Limit Switch | Accident trigger |
| LED | Emergency indicator |
| Power Supply & Wires | System power |

---

## 4. System Architecture
## System Architecture

![Smart Helmet Architecture](assets/System_Architecture.png)


---

## 5. Circuit Connection Guide

| Module | Arduino Pin |
|--------|-------------|
| GPS TX/RX | D2 / D3 |
| GSM TX/RX | D8 / D7 |
| Tilt Sensor | A1 |
| Limit Switch | D4 (INPUT_PULLUP) |
| LED | D13 |

---

## 6. Working Principle

1. Helmet continuously reads sensor values
2. If tilt > threshold OR limit switch pressed:
   - Read current GPS coordinates
   - Generate emergency alert
   - SMS alert sent with real-time location
3. LED blinks during alert mode

---

## 7. Arduino Code

> Refer to the `SmartHelmet.ino` file in this repository  
(Place the updated code here in your repo)

---

## 8. SMS Alert Format

Example SMS received:


Block Diagram (upload image here later)

