# 🚀 AI Powered Predictive Life Monitoring for Machine Critical Spares

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-Zero%202W-C51A4A?logo=raspberrypi)
![Unity](https://img.shields.io/badge/Unity-2022-black?logo=unity)
![MQTT](https://img.shields.io/badge/MQTT-EMQX-orange)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-green)

A real-time predictive maintenance system for conventional lathe machines developed using **Raspberry Pi Zero 2 W**, **IoT sensors**, **Machine Learning**, **MQTT**, and a **Unity-based Digital Twin**.

The system continuously monitors machine vibration and temperature from the tailstock region, processes the collected data locally on the Raspberry Pi, predicts machine health using a trained Random Forest model, estimates the Remaining Useful Life (RUL), and visualizes the results through an interactive Unity dashboard and Android application.

---

# 📌 Project Overview

Conventional lathe machines are generally maintained using reactive or scheduled maintenance strategies, which often result in unexpected machine failures, increased maintenance costs, and production downtime. This project presents a low-cost predictive maintenance solution capable of continuously monitoring machine condition and identifying abnormal behaviour before critical failures occur.

The Raspberry Pi Zero 2 W acts as the edge computing device, collecting vibration and temperature data from the ADXL345 and DS18B20 sensors. After preprocessing and feature extraction, a machine learning model predicts the machine condition and estimates its Remaining Useful Life (RUL). The processed information is transmitted using MQTT and visualized in real time through a Unity-based Digital Twin and Android application.

---

# ✨ Features

- Real-time vibration monitoring using ADXL345
- Real-time temperature monitoring using DS18B20
- Raspberry Pi Zero 2 W edge processing
- Signal preprocessing and feature extraction
- Machine Learning-based fault classification
- Remaining Useful Life (RUL) estimation
- MQTT-based real-time communication
- Unity Digital Twin Dashboard
- Android APK for portable monitoring
- Live machine condition visualization
- Visual fault indication

---

# 🏗 System Architecture

```
             ADXL345              DS18B20
                │                    │
                └──────────┬─────────┘
                           │
                Raspberry Pi Zero 2 W
                           │
      Signal Processing & Feature Extraction
                           │
             Random Forest Prediction
                           │
                   MQTT Communication
                           │
      Unity Digital Twin Dashboard / Android APK
```

---

# 🔄 Workflow

```
Sensor Data Collection
          │
          ▼
Signal Preprocessing
          │
          ▼
Feature Extraction
          │
          ▼
Machine Learning Prediction
          │
          ▼
Remaining Useful Life Estimation
          │
          ▼
MQTT Data Publishing
          │
          ▼
Unity Digital Twin Visualization
```

---

# 🛠 Hardware Used

| Component | Description |
|------------|-------------|
| Raspberry Pi Zero 2 W | Edge Computing Device |
| ADXL345 | 3-Axis Digital Accelerometer |
| DS18B20 | Digital Temperature Sensor |

---

# 💻 Software & Technologies

- Python
- Raspberry Pi OS Lite (64-bit)
- Unity Engine
- MQTT (EMQX Broker)
- Scikit-learn
- Pandas
- NumPy
- Paho MQTT
- Git & GitHub

---

# 💻 System Requirements

- Raspberry Pi Zero 2 W
- Raspberry Pi OS Lite (64-bit)
- Python 3.11 or later
- Unity 2022 LTS
- EMQX MQTT Broker

---

# 📂 Project Structure

```
AI-Powered-Predictive-Maintenance-for-Critical-Machine-Spares-in-CNC-Lathe-Machines/
│
├── raspberry_pi/
│   ├── s_v.py
│   ├── requirements.txt
│   ├── lathe_model.pkl
│   └── sv.service
│
├── unity_dashboard/
│   ├── Assets/
│   ├── Scripts/
│   └── Scenes/
│
├── mobile_apk/
│
├── datasets/
│
├── docs/
│
├── images/
│
└── README.md
```

---

# ⚙ Installation

### Clone the Repository

```bash
git clone https://github.com/Sanjay67789/AI-Powered-Predictive-Maintenance-for-Critical-Machine-Spares-in-CNC-Lathe-Machines.git

cd AI-Powered-Predictive-Maintenance-for-Critical-Machine-Spares-in-CNC-Lathe-Machines
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Raspberry Pi Application

```bash
python s_v.py
```

### Launch Unity Dashboard

Open the Unity project and connect it to the configured MQTT broker.

---

# 📡 MQTT Topics

| Topic | Description |
|---------|-------------|
| vibration/1 | Vibration Sensor Data |
| temp/1 | Temperature Sensor Data |

---

# 🤖 Machine Learning

The vibration signal collected from the ADXL345 sensor undergoes preprocessing and feature extraction before being analyzed using a Random Forest classifier.

### Extracted Features

- Ax Standard Deviation
- Ay Standard Deviation
- Az Standard Deviation
- Ax Range
- Ay Range
- Az Range

### Machine States

- ✅ Healthy
- ⚠ Warning
- 🔴 Critical

The system also estimates the Remaining Useful Life (RUL) using vibration trend analysis.

---

# 🖥 Unity Digital Twin

The Unity application functions as a Digital Twin of the physical lathe machine by providing an intuitive visualization of real-time machine behaviour.

### Dashboard Features

- Live vibration monitoring
- Temperature monitoring
- Machine health status
- Remaining Useful Life (RUL)
- Visual fault indication
- Interactive Digital Twin
- Android APK deployment

---

# 📱 Android Application

The Unity project is also deployed as an Android APK, allowing users to monitor the machine remotely through a mobile device.

---

# 📊 Output

The developed system successfully provides

- Real-time vibration monitoring
- Real-time temperature monitoring
- Machine health prediction
- Remaining Useful Life estimation
- MQTT communication
- Unity Digital Twin visualization
- Android-based monitoring

---

# 🎯 Skills Demonstrated

- Embedded Systems
- Raspberry Pi
- IoT
- Sensor Interfacing
- MQTT Communication
- Machine Learning
- Predictive Maintenance
- Digital Twin
- Unity Development
- Python Programming
- Edge Computing

---

# 📸 Screenshots

Add screenshots inside the **images** folder.

Example:

```
<img width="1028" height="593" alt="WPS Photos(1)" src="https://github.com/user-attachments/assets/2e3291a3-45d1-4202-ad20-2f84b7d4b0c8" />
 -Lathe Mchine setup
<img width="628" height="355" alt="image" src="https://github.com/user-attachments/assets/31b42e1b-143f-4c12-9f1c-fb47286cba1a" />
-Unity 3d
<img width="620" height="273" alt="image" src="https://github.com/user-attachments/assets/833376b4-1b39-4d5c-b353-e536700372ab" />
-Android APK

```

---

# 🚀 Future Enhancements

- Multi-machine monitoring
- Cloud dashboard integration
- Deep Learning-based fault prediction
- Historical data analytics
- Remote notification system
- Additional industrial sensors
- Web dashboard support

---

# 👨‍💻 Team

### Project Title

**AI Powered Predictive Life Monitoring for Machine Critical Spares**

### Developed By

- **Sanjay Kumar P** *(Team Lead)*
- **Premkumar A**
- **Rich Jewin A M**

---

# 📌 Project Status

**✅ Completed**

Developed as an undergraduate engineering project demonstrating the practical implementation of AI-assisted predictive maintenance using Raspberry Pi, Machine Learning, MQTT, and Unity Digital Twin technology.

---

# 📜 License

This project is developed for educational and research purposes.

---

# 📬 Contact

**Sanjay Kumar P**

📧 Email: **sanjayk67789@gmail.com**

🐙 GitHub: **https://github.com/Sanjay67789**
