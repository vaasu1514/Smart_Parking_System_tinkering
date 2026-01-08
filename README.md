# Smart Parking System using NodeMCU (ESP8266)

## Overview
This project implements an **IoT-based smart parking system** that detects vehicle presence in parking slots and provides **real-time availability updates** using cloud connectivity. The system uses **NodeMCU (ESP8266)**, **IR sensors**, and **Firebase** to connect hardware with a mobile application for live parking status monitoring.

---

## System Architecture
The system is built using two ESP8266 NodeMCU boards:
- One controller handles **IR sensor inputs** and **servo motor gate control**
- A second controller manages **LED indicators** and **cloud communication**

Both controllers communicate through **Firebase Realtime Database**, ensuring consistent parking status updates across hardware and the mobile app.

---

## Hardware Components
- NodeMCU (ESP8266) × 2  
- Infrared (IR) Sensors × 5  
- Servo Motor (gate control)  
- LEDs (slot status indicators)  
- Breadboard and jumper wires  

---

## Software & Tools
- **Arduino IDE** – Firmware development for ESP8266  
- **Firebase Realtime Database** – Cloud backend for parking data  
- **Android Studio** – Mobile application interface  
- **Wi-Fi (ESP8266)** – Real-time data transmission  

---

## Key Features
- Vehicle detection using **IR sensors** for each parking slot  
- Real-time slot availability updates via **Firebase**  
- LED indicators reflecting live parking status  
- Servo-based gate control for vehicle entry  
- Mobile application displaying occupied and available slots  

---

## Challenges & Solutions
- **LED status mismatch due to communication delays**  
  → Implemented feedback logic to update LEDs using the latest Firebase data  

- **Limited GPIO availability on a single ESP8266**  
  → Distributed functionality across two NodeMCU boards  

- **Controlled vehicle entry requirement**  
  → Integrated **QR-code–based access verification** linked with Firebase data  

---

## Repository Contents
- `README.md` – Project documentation  
- `TINKERING (1).pdf` – Detailed project report with circuit diagrams and results  

---

## My Contributions
- Implemented Wi-Fi connectivity and Firebase integration  
- Enabled live parking status updates from hardware to mobile application  
- Verified real-time data flow between sensors, cloud, and app  

---

