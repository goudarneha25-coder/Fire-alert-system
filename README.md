# 🔥 IoT Fire Alert System

A real-time IoT-based Fire and Gas Monitoring System using ESP8266, Firebase Realtime Database, and a Live Web Dashboard deployed on Vercel.

---

## 📌 Project Overview

This project detects fire and gas leakage using sensors connected to an ESP8266 microcontroller.  
Sensor data is sent to Firebase Realtime Database and displayed live on a web dashboard.

The system provides:
- Real-time gas level monitoring
- Fire detection status
- Threshold-based alerts
- Live web dashboard visualization

---

## 🛠️ Hardware Components

- ESP8266 (NodeMCU)
- MQ Gas Sensor
- Flame Sensor
- Buzzer
- Jumper Wires
- Breadboard
- Power Supply

---

## 🧠 System Architecture

ESP8266 reads sensor data →  
Sends data to Firebase →  
Web Dashboard fetches live data from Firebase →  
Displays real-time alerts.

---

## 🔥 Firebase Realtime Database Structure

```
fire-alert-d5570-default-rtdb
│
├── gasLevel: number
├── fireStatus: boolean
├── threshold: number
├── alertTime: string
```

---

## 💻 ESP8266 Arduino Code

The ESP8266:
- Connects to WiFi
- Sends sensor values to Firebase
- Triggers buzzer if gas exceeds threshold

Main Functions:
- Read MQ gas sensor value
- Detect flame sensor state
- Update Firebase fields:
  - gasLevel
  - fireStatus
  - alertTime

---

## 🌐 Web Dashboard

The dashboard:
- Fetches live data from Firebase
- Displays gas level
- Shows fire detection status
- Updates automatically in real-time

### Technologies Used:
- HTML
- CSS
- JavaScript
- Firebase Web SDK

---

## 🚀 Live Deployment

🔗 Live Dashboard:  
https://iot-fire-alert-system.vercel.app

Hosted using **Vercel**.

---

## 📂 Project Structure

```
IoT-Fire-Alert-System
│
├── index.html
├── style.css
├── script.js
├── ESP8266_Code.ino
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Hardware Setup
- Connect MQ gas sensor to analog pin
- Connect flame sensor to digital pin
- Connect buzzer to output pin

### 2️⃣ Firebase Setup
- Create Firebase project
- Enable Realtime Database
- Copy:
  - Database URL
  - API Key
  - Project ID
- Update in:
  - ESP8266 code
  - script.js

### 3️⃣ ESP8266 Setup
- Install ESP8266 board in Arduino IDE
- Install required libraries:
  - ESP8266WiFi
  - Firebase ESP Client
- Upload code to board

### 4️⃣ Deploy Web Dashboard
- Push project to GitHub
- Import repository into Vercel
- Deploy

---

## 🎯 Features

✔ Real-time monitoring  
✔ Firebase cloud integration  
✔ Web-based dashboard  
✔ IoT-based fire alert  
✔ Gas threshold detection  

---

## 📸 Future Improvements

- SMS alert system
- Email notification
- Mobile app integration
- Historical data storage
- Graph visualization

---

## 👨‍💻 Author

Developed as an IoT project using ESP8266 and Firebase.

---

## 📜 License

This project is for educational purposes.
