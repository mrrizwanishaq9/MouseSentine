# 🛡️ MouseSentinel V23

**MouseSentinel V23** is a professional Python-based Windows PC security and privacy monitoring tool. It helps monitor local activity, detect inactivity and newly connected USB storage devices, capture optional webcam evidence, trigger security alerts, encrypt event logs, and generate security reports.

> ⚠️ **Defensive-use project:** Designed for protecting and monitoring your own Windows computer. It does not capture typed passwords or perform stealth keylogging.

## ✨ Features

* 🖱️ Mouse activity monitoring
* ⌨️ Keyboard activity counting without storing typed text
* ⏱️ Inactivity detection and auto-lock option
* 🔌 USB storage device detection
* 📷 Optional webcam snapshot capture
* 👤 Basic webcam face-presence detection
* 🔊 Security alarm
* 🔔 Desktop notifications
* 🔐 PIN-protected settings
* 🔒 Windows native workstation lock
* 🛡️ Encrypted security event logs
* 📊 Security dashboard and score
* 📄 TXT/CSV security reports
* 🧪 Safe Test Mode
* ⚙️ Configurable security settings
* 🚀 Optional Windows startup support
* 🗂️ Automatic logs, captures, reports, and configuration folders

## 🧰 Technologies

* Python 3.13
* Tkinter
* OpenCV
* psutil
* pynput
* Cryptography / Fernet
* PowerShell
* Windows API

## 📦 Installation

Recommended Python version:

```text
Python 3.13
```

Install dependencies:

```powershell
py -3.13 -m pip install psutil pynput opencv-python cryptography plyer
```

## ▶️ Run

Open PowerShell in the project directory:

```powershell
cd "C:\Users\Dell\Desktop\pythonvs"
```

Then run:

```powershell
py -3.13 mousesentinel_v23.py
```

If your file is inside `.vscode`:

```powershell
cd "C:\Users\Dell\Desktop\pythonvs\.vscode"
py -3.13 mousesentinel_v23.py
```

## 🧪 Safe Test Mode

MouseSentinel starts with **Safe Test Mode enabled**. This allows you to test monitoring, camera capture, USB detection, notifications, alarms, and logging without automatically locking Windows.

After testing, you can configure the protection settings according to your needs.

## 📁 Data Structure

MouseSentinel automatically creates:

```text
MouseSentinel/
├── captures/
├── logs/
│   └── security_events.enc
├── reports/
├── config.json
└── secret.key
```

## 🔐 Security

Security events can be stored using Fernet encryption. The application uses a salted PBKDF2-HMAC-SHA256 process for its local PIN protection.

MouseSentinel does **not** store actual keyboard characters or passwords.

## 📊 Example Monitoring

```text
========================================
       MouseSentinel V23
========================================

Status:              PROTECTED
Safe Test Mode:      ON
Mouse Events:        128
Keyboard Events:     74
Inactivity:          00:12
USB Devices:         2
CPU Usage:           18%
RAM Usage:           46%
Battery:             82%
Security Score:      94/100
========================================
```

## ⚠️ Limitations

* Webcam face checking is basic face-presence detection, not biometric identity verification.
* USB monitoring primarily targets USB storage devices.
* Camera access requires Windows camera permission.
* Windows locking is handled by the native Windows security system.
* Some notification features are optional depending on installed packages.

## 🎯 Project Goal

MouseSentinel V23 is designed as a practical Python cybersecurity and privacy project for learning **Windows security monitoring, automation, GUI development, event detection, encryption, system monitoring, and defensive security engineering**.

## 👨‍💻 Author

**Muhammad Rizwan**

Python • AI • Robotics • Cybersecurity Learning

## 📜 License

This project is intended for educational and defensive security purposes. Use it only on computers and systems you own or have explicit permission to monitor.
