# IAQ-Monitoring

# 🌿 IAQ Monitoring System (Flutter + Firebase + ThingSpeak)

This IAQ (Indoor Air Quality) Monitoring System tracks and displays real-time indoor air metrics like temperature, humidity, PM2.5, VOCs, and CO₂ levels. It uses environmental sensors to collect data, uploads it to ThingSpeak, and fetches and visualizes it through a Flutter-based mobile application with Firebase integration for user management and optional data logging.

---

## 📱 Features

- Real-time air quality display using ThingSpeak APIs
- Graphical sensor data visualization (charts)
- Firebase Authentication (Login/Signup)
- Firebase Firestore for optional data storage/logs
- Alert system for poor air quality
- Clean, responsive UI

---

## 🔧 Prerequisites

1. Hardware
   - ESP32 or NodeMCU board
   - MQ135 (gas sensor), DHT11/22, PMS5003 (optional for PM2.5)
   - Breadboard, wires, 5V power supply

2. Software & Tools
   - Flutter SDK
   - Dart
   - Firebase account (Firestore, Auth enabled)
   - ThingSpeak account (channel + API key)
   - Android Studio / VS Code

3. Flutter Packages
   - http
   - firebase_core
   - firebase_auth
   - cloud_firestore
   - fl_chart (for graphs)
   - provider / riverpod (for state management, optional)

---

## 🚀 Setup Instructions

 1. Hardware
- Upload Arduino code to ESP32/NodeMCU to collect sensor data
- Use Wi-Fi to send data to ThingSpeak using its API (write API key)
- Set ThingSpeak to public/private depending on use

 2.Dependencies
 dependencies:
  flutter:
    sdk: flutter
  http: ^0.14.0
  firebase_core: ^2.0.0
  firebase_auth: ^4.0.0
  cloud_firestore: ^4.0.0
  fl_chart: ^0.50.0
  provider: ^6.0.0  # if you're using provider for state management



 3. Flutter App Setup
```bash
flutter pub get
flutter run

