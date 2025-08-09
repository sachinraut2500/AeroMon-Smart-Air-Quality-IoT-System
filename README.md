# AeroMon – Smart Air Quality IoT System

**AeroMon** is a Python-based IoT simulation project that models a distributed **air quality monitoring network**.  
It uses **MQTT** for real-time telemetry, stores readings in **SQLite**, calculates **AQI (Air Quality Index)**, detects anomalies, and provides a **REST API** + **dashboard**.

---

## 🚀 Features
- **Simulated IoT Nodes**  
  Multiple virtual sensors broadcasting **temperature**, **humidity**, **CO₂**, and **PM2.5** readings.
- **MQTT Communication**  
  Device-to-cloud data transfer via [test.mosquitto.org](https://test.mosquitto.org) public broker.
- **SQLite Data Storage**  
  Local time-series database for telemetry history.
- **AQI Calculation**  
  Automatic categorization of PM2.5 readings into standard AQI ranges.
- **Real-Time REST API**  
  `/recent` endpoint to retrieve the latest readings.
- **Dashboard Generation**  
  PM2.5 trend chart using Matplotlib.
- **Colab-Ready**  
  Runs directly in Google Colab with auto-installation of dependencies.

---

## 🛠 Requirements
- Python 3.8+
- Internet connection (for MQTT broker)
- Dependencies (auto-installed in Colab or run locally):
  - `paho-mqtt`
  - `flask`
  - `matplotlib`

---

## 📦 Installation

### 1. Clone this repo
```bash
git clone https://github.com/<your-username>/aeromon.git
cd aeromon
