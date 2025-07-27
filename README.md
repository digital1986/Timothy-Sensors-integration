 [![Link to Video](https://arduinointro.com/images/piezo/piezo_ultrasonic/piezo-ultrasonic-cover-900.jpg)](https://www.youtube.com/shorts/MIEfrskdpz0)



# Ultrasonic Obstacle Detector with Buzzer and Temperature Sensor (Raspberry Pi)

This project combines an ultrasonic sensor, a line tracker, a buzzer, and a DHT22 temperature/humidity sensor using a Raspberry Pi. The system detects nearby obstacles and environmental conditions, then activates a buzzer if necessary.

---

## 📦 Components Used

- Raspberry Pi (GPIO support)
- HC-SR04 Ultrasonic Distance Sensor
- DHT22 Temperature & Humidity Sensor
- Line Tracker Sensor
- Buzzer
- Python 3
- Adafruit_DHT Library

---

## 🚀 Features

- 🔊 Sounds a buzzer if an object is closer than 10 cm.
- 📏 Measures distance using an ultrasonic sensor.
- 🌡️ Reads temperature and humidity via DHT22.
- 🧲 Uses a tracker sensor to detect objects on a surface.
- 🧼 Graceful cleanup of GPIO on interruption.

---

## 🛠️ Setup Instructions

### 1. Hardware Connections

| Component        | GPIO Pin (BCM) | Notes                          |
|------------------|----------------|--------------------------------|
| Ultrasonic TRIG  | 23             | Output                         |
| Ultrasonic ECHO  | 24             | Input                          |
| Buzzer           | 21             | Output                         |
| DHT22 Sensor     | 22             | Data pin, uses Adafruit_DHT    |
| Tracker Sensor   | 2              | Input pin                      |

### 2. Install Dependencies

```bash
git clone https://github.com/digital1986/Timothy-Sensors-integration
sudo apt-get update
sudo apt-get install python3-pip
pip3 install Adafruit_DHT
```

> Ensure `RPi.GPIO` is installed (usually pre-installed on Raspbian):
```bash
pip3 install RPi.GPIO
```

### 3. Run the Script

```bash
python3 altrasonic_obstacle_buzzer_temp.py
```

Press `Ctrl+C` to stop the script.

---

## 📁 File Descriptions

- `altrasonic_obstacle_buzzer_temp.py`: Main Python script containing all logic.
- `requirements.txt`: Python dependencies.
- `.gitignore`: Files to ignore in GitHub (e.g., `.pyc`, `__pycache__`).
- `README.md`: Project documentation.

---
---

## 👤 Author

**Your Name** Timothy Nwadike  
[GitHub Profile](https://github.com/digital1986/Timothy-Sensors-integration.git)

---
