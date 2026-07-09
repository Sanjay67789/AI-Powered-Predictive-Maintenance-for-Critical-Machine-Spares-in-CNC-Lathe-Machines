# 🚀 AI Powered Predictive Life Monitoring for Machine Critical Spares

A real-time predictive maintenance system developed for conventional lathe machines using **Raspberry Pi Zero 2 W**, **IoT sensors**, **Machine Learning**, **MQTT**, and a **Unity-based Digital Twin**.

The system continuously monitors the condition of the lathe machine by acquiring vibration and temperature data from the tailstock region. The collected data is processed locally on the Raspberry Pi, analyzed using a machine learning model, and visualized in real time through an interactive Unity dashboard and Android application.

---

## 📌 Project Overview

Traditional lathe machines are generally maintained using reactive or scheduled maintenance, which often leads to unexpected failures and production downtime. This project introduces a low-cost predictive maintenance solution capable of detecting abnormal machine behavior before major failures occur.

The system performs real-time monitoring using vibration and temperature sensors, predicts machine condition using machine learning, estimates Remaining Useful Life (RUL), and presents all information through a digital twin dashboard.

---

## ✨ Features

- Real-time vibration monitoring using ADXL345
- Temperature monitoring using DS18B20
- Raspberry Pi Zero 2 W edge processing
- MQTT-based real-time communication
- Machine Learning-based fault classification
- Remaining Useful Life (RUL) estimation
- Unity Digital Twin Dashboard
- Android APK for mobile monitoring
- Live machine status visualization
- Fault indication using visual alerts

---

# 🏗 System Architecture

```
                ADXL345            DS18B20
                   │                  │
                   └──────────┬───────┘
                              │
                     Raspberry Pi Zero 2 W
                              │
               Signal Processing & Feature Extraction
                              │
                    Machine Learning Prediction
                              │
                       MQTT Communication
                              │
              Unity Digital Twin Dashboard / Android APK
```

---

# 🔄 Workflow

```
Sensor Data Collection
          ↓
Signal Preprocessing
          ↓
Feature Extraction
          ↓
Machine Learning Prediction
          ↓
Remaining Useful Life Estimation
          ↓
MQTT Data Publishing
          ↓
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
- Raspberry Pi OS
- Unity
- MQTT
- Machine Learning
- Scikit-learn
- Pandas
- NumPy
- Paho MQTT
- Git

---

# 📂 Project Structure

```
AI-Powered-Predictive-Life-Monitoring/
│
├── raspberry_pi/
│   ├── s_v.py
│   ├── requirements.txt
│   └── lathe_model.pkl
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
├── images/
│
├── docs/
│
└── README.md
```

---

# ⚙ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI-Powered-Predictive-Life-Monitoring.git

cd AI-Powered-Predictive-Life-Monitoring
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the Raspberry Pi application

```bash
python s_v.py
```

Launch the Unity dashboard and connect it to the MQTT broker.

---

# 📡 MQTT Topics

| Topic | Description |
|---------|-------------|
| vibration/1 | Vibration Data |
| temp/1 | Temperature Data |

---

# 🤖 Machine Learning

The collected vibration signal undergoes preprocessing and feature extraction before being analyzed using a Random Forest model.

Extracted Features include:

- Ax Standard Deviation
- Ay Standard Deviation
- Az Standard Deviation
- Ax Range
- Ay Range
- Az Range

The model classifies machine condition into:

- Healthy
- Warning
- Critical

The system also estimates the Remaining Useful Life (RUL) based on vibration trends.

---

# 🖥 Unity Dashboard

The Unity dashboard functions as a Digital Twin of the physical lathe machine.

It provides:

- Live vibration values
- Temperature monitoring
- Machine status
- Fault indication
- Remaining Useful Life
- Interactive user interface
- Android APK deployment

---

# 📱 Android Application

The Unity project is exported as an Android APK, enabling portable monitoring of machine condition through a smartphone.

---

# 📸 Screenshots

> Add screenshots inside the `images` folder and reference them here.

Example:

```
images/dashboard.png
images/setup.jpg
images/mobile_app.png
images/fault_detection.png
```

---

# 🚀 Future Enhancements

- Multi-machine monitoring
- Cloud integration
- Advanced Deep Learning models
- Additional industrial sensors
- Historical analytics dashboard
- Predictive maintenance notifications

---

# 👨‍💻 Team

**Project Title**

AI Powered Predictive Life Monitoring for Machine Critical Spares

**Developed By**

- Sanjay Kumar P
- Premkumar A
- Rich Jewin A M

---

# 📜 License

This project is developed for academic and research purposes.

---


## 📬 Contact

**Sanjay Kumar**
- Email : sanjayk67789@gmail.com
