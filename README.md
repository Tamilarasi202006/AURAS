# 🚨 AURAS - Ambulance Urgency Response & Alert System

AURAS is a lightweight real-time alert system designed to notify nearby police or emergency responders when an ambulance or individual is in distress. This system uses geolocation and Firebase to send live alerts that can be viewed on a centralized dashboard.

## 🚀 Project Overview

During emergency situations, seconds can save lives. AURAS ensures faster response times by bridging the communication gap between the public (or ambulance drivers) and the authorities.

## 🧠 Features

- 🔴 **Emergency Alert Button** for quick notification
- 🌐 **Geolocation Support** to share the real-time location
- ☁️ **Firebase Real-Time Database** to sync alert data instantly
- 👮 **Live Dashboard for Police/Responders** to monitor emergency reports

## 📁 Project Structure

- `auras.html`: Webpage used by the driver or public to send emergency alerts with location data.
- `police.html`: Live dashboard for police to monitor incoming emergency alerts in real time.

## 🔧 Technologies Used

- HTML5, JavaScript
- Firebase (Realtime Database)
- Geolocation API

## 📸 Demo video
https://youtu.be/rPklhGT3bHE


## 🛠️ How It Works

1. User clicks on **🔴 Alert Police** button in `auras.html`.
2. Geolocation coordinates are captured via browser.
3. Data is pushed to Firebase (`ambulanceAlerts` node).
4. `police.html` listens for changes and displays the alert in real time.

## 🧪 How to Run

1. Clone the repository
   ```bash
git clone https://github.com/Tamilarasi202006/auras.git
Firebase Setup
Replace the Firebase config objects in both HTML files with your own Firebase credentials:
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};
