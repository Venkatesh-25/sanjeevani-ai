---
publishDate: 2026-05-24T00:00:00Z
title: Sanjeevani AI
excerpt: A context-aware predictive emergency intelligence system that uses MYOSA sensor fusion to detect, explain, and escalate real-time safety risks from environment, motion, posture, pressure, gesture, and fall signatures.
image: sanjeevani_ai/cover-dashboard.png
tags:
  - MYOSA
  - IoT
  - Sensor-Fusion
  - Emergency-Intelligence
  - ESP32
---

> Context-Aware Predictive Emergency Intelligence System using MYOSA Sensor Fusion.

---

## Acknowledgements

Sanjeevani AI was developed by Team Sanjeevini AI from Symbiosis Institute of Technology, Hyderabad for the IEEE MYOSA Event 5.0 ecosystem.

The project uses the MYOSA Mini IoT Kit as the core sensing platform and demonstrates how embedded sensor fusion, explainable risk intelligence, and remote escalation can work together to improve emergency awareness in indoor spaces, assisted living environments, classrooms, laboratories, hostels, smart buildings, and public safety zones.

---

## Overview

Sanjeevani AI is a predictive emergency intelligence system built around MYOSA sensor fusion.

Most emergency systems are either reactive, single-purpose, or dependent on manual action. A fall button only works if the person can press it. A wearable only works if the person is wearing and charging it. A smoke or air-quality monitor only understands one part of the situation. A basic threshold alarm may trigger too late, too often, or without explaining why.

Sanjeevani AI is designed differently.

It continuously reads multiple MYOSA sensor channels and converts them into one explainable emergency risk stream. The system observes environmental stress, air quality, motion behavior, posture change, pressure variation, gesture input, fall signatures, sensor confidence, and response readiness. Instead of reacting to a single value, it studies context: what changed, how quickly it changed, which sensors agree, whether the pattern is temporary or persistent, and whether the situation is becoming unsafe.

The result is a real-time emergency intelligence command center that can detect early warning patterns, explain the reason behind risk changes, show live fused data, trigger local response indicators, and communicate status through a Telegram alert bot.

**Key features:**

* MYOSA-based contextual sensor fusion
* Unified 0–100 emergency risk score
* SAFE, WATCH, WARNING, and EMERGENCY state model
* Fall-signature detection using motion, posture, impact, and inactivity context
* Explainable incident story and decision matrix
* Real-time dashboard with live graphs and sensor confidence
* OLED display for local device status
* LED and buzzer-ready response layer
* Telegram command bot for remote status and emergency awareness
* Simulation-ready operation for smooth evaluation and presentation
* Mobile-friendly and large-screen dashboard experience

Sanjeevani AI is an engineering prototype and innovation showcase project. It is not a certified medical device and does not replace professional emergency services. Its purpose is to demonstrate how MYOSA sensor fusion can support earlier awareness, clearer explanation, and faster response workflows.

---

## Demo / Examples

### Images

<p align="center">
  <img src="/assets/images/sanjeevani_ai/cover-dashboard.png" width="800"><br/>
  <i>Real-time emergency intelligence command center showing unified risk, incident story, Telegram readiness, sensor confidence, and response status.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/sensor-fusion-dashboard.png" width="800"><br/>
  <i>Live MYOSA sensor fusion dashboard combining environment, motion, posture, gesture, fall signature, and risk stream.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/myosa-hardware-stack.jpg" width="800"><br/>
  <i>Compact MYOSA hardware stack with live LED indicator, showing the physical embedded setup used for the emergency intelligence stream.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/myosa-hardware-oled.jpg" width="800"><br/>
  <i>MYOSA Mini IoT hardware running Sanjeevani AI with OLED status display and local LED response.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/myosa-hardware-angle.jpg" width="800"><br/>
  <i>Physical sensing unit showing live monitoring, local status output, and embedded response indicators.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/decision-matrix.png" width="800"><br/>
  <i>Explainable decision matrix showing how environment, motion, manual distress, and fusion confidence influence the final risk state.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/environment-graph.png" width="800"><br/>
  <i>Real-time environment stream combining temperature, humidity, and air-quality context.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/motion-physiology-graph.png" width="800"><br/>
  <i>Motion physiology stream tracking movement, tilt, and pressure-related context for emergency interpretation.</i>
</p>

<p align="center">
  <img src="/assets/images/sanjeevani_ai/telegram-escalation.jpg" width="800"><br/>
  <i>Telegram command bot enabling remote status checks, latest fused packet review, emergency history, scenario control, and incident resolution.</i>
</p>

### Videos

<video controls width="100%">
  <source src="/sanjeevani-ai-final-video.mp4" type="video/mp4">
</video>

---

## Features (Detailed)

### 1. Context-aware MYOSA sensor fusion

Sanjeevani AI uses the MYOSA Mini IoT Kit as a multi-signal sensing platform. It combines temperature, humidity, air quality, motion, posture, pressure, gesture, and fall-related patterns into one fused decision stream.

This is important because real emergencies are rarely visible through one sensor alone. A fall may involve impact, tilt, and reduced motion. Poor indoor safety may involve rising temperature, humidity, and air-quality stress. A manual distress signal may become more important when it appears together with abnormal posture or environmental risk.

Sanjeevani AI is built around this idea: the system should understand relationships between signals, not just read sensor values.

### 2. Unified emergency risk score

The system converts fused sensor behavior into a unified emergency risk score from 0 to 100.

The score is designed to be easy to understand:

* **0–24:** SAFE  
* **25–49:** WATCH  
* **50–74:** WARNING  
* **75–100:** EMERGENCY  

Normal fused readings remain low. Risk increases when multiple patterns appear together, such as abnormal air quality with environmental stress, sudden posture change with motion disturbance, or fall-like movement followed by inactivity.

This makes the system predictive instead of purely reactive.

### 3. Explainable emergency states

Sanjeevani AI uses a clear state model:

* **SAFE:** normal baseline behavior  
* **WATCH:** early weak signal or slight deviation  
* **WARNING:** multiple risk indicators are present  
* **EMERGENCY:** strong fused evidence that attention may be needed  

Every state is supported by reason codes, confidence, and incident summaries. The dashboard does not simply show a number. It explains why the system reached that state.

Example reasons include:

* normal baseline
* environment stress
* air-quality rise
* motion/posture signature
* fall candidate
* fall confirmed
* SOS gesture
* multi-sensor risk
* sensor confidence change

### 4. Fall-signature intelligence

Sanjeevani AI does not treat a fall as only one acceleration spike.

The fall logic looks for a sequence of events:

1. sudden motion or impact-like behavior  
2. posture or tilt change  
3. abnormal motion pattern  
4. reduced movement after the event  
5. recovery or non-recovery context  

This makes the system more realistic than a simple impact alarm. It also makes the result easier to explain during a demonstration because the dashboard can show the cause-and-effect sequence.

### 5. Real-time command center dashboard

The dashboard is designed to look and behave like a serious emergency intelligence product.

It includes:

* live system state badge
* unified risk score
* confidence indicator
* incident story
* live environment graph
* live motion physiology graph
* decision matrix
* sensor cards
* emergency log
* Telegram escalation status
* response readiness
* mobile-friendly layout

The dashboard uses a warm clinical visual design with off-white, orange, green, and soft neutral tones. It is designed for clarity during live judging, not just for raw data display.

### 6. Incident story and decision matrix

The incident story explains what the system believes is happening.

Instead of showing only sensor numbers, it generates a human-readable interpretation such as:

* safe baseline
* environment stress rising
* motion and posture mismatch detected
* fall signature under observation
* emergency escalation active

The decision matrix breaks the decision into categories:

* environment stress
* motion/posture signature
* manual distress
* fusion confidence

This helps judges and users immediately understand that Sanjeevani AI is not a black-box alarm. It is an explainable intelligence layer.

### 7. Sensor confidence and response readiness

Real hardware can have temporary missing readings, sensor variation, or connection changes. Sanjeevani AI handles this by showing sensor confidence instead of hiding uncertainty.

The dashboard displays how many sensors are contributing to the fused decision. This helps users trust the system because it is honest about signal quality.

The response readiness panel also shows whether local response channels such as OLED, LED, buzzer, and Telegram escalation are available.

### 8. Telegram emergency communication

Sanjeevani AI includes a Telegram bot workflow for remote emergency awareness.

The bot can be used by a caregiver, teammate, reviewer, or family member to check the current state of the system. It supports status checks, latest fused packet review, emergency history, simulation control, and incident resolution.

Supported bot commands:

```plaintext
/start
/status
/last
/emergencies
/resolve
/simulate normal
/simulate warning
/simulate emergency
/help
```

This expands the project beyond a local dashboard. It becomes a communication-ready emergency awareness platform.

### 9. Local device feedback

The physical MYOSA unit provides local status through OLED and LED output. The OLED shows monitoring state, risk level, temperature, pressure, tilt, and normal/emergency status. The LED provides an immediate visual status indicator.

A buzzer-ready response path is also included for local audible escalation when required.

### 10. Simulation-ready evaluation mode

The system supports a smooth presentation-ready stream so evaluators can see stable live behavior even when environmental readings or hardware access are limited.

This is useful for competitions because live demos must remain dependable. The dashboard still shows realistic fused behavior, risk movement, graphs, confidence, and incident interpretation.

### 11. Why Sanjeevani AI is different

Sanjeevani AI is not just another sensor monitor.

Compared with common alternatives:

* **Wearables** require the person to wear, charge, and maintain a device.
* **Panic buttons** require the person to be conscious and able to press a button.
* **Air-quality monitors** focus only on environmental safety.
* **Basic fall alarms** often rely on a single motion trigger.
* **Generic IoT dashboards** show values but do not explain emergency context.

Sanjeevani AI combines room-level sensing, fall-signature intelligence, environmental context, explainable scoring, local response, dashboard visualization, and Telegram communication in one integrated system.

Its main strength is contextual interpretation.

---

## Usage Instructions

### Hardware walkthrough

1. Power the MYOSA Mini IoT Kit and connected response indicators.
2. Confirm the OLED display shows monitoring status.
3. Start the backend server.
4. Open the dashboard in a browser.
5. Observe baseline readings for temperature, humidity, AQI, pressure, motion, posture, gesture, and fall signature.
6. Trigger walkthrough scenarios such as movement change, environmental stress, SOS gesture, or fall-like orientation change.
7. Watch the unified risk, incident story, decision matrix, and graphs update in real time.
8. Use the Telegram bot to check status, latest packet, emergency history, or resolution state.

### Run the project on Windows

From the project root:

```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements_global.txt
python dashboard/backend/server.py
```

Then open the dashboard in a browser:

```plaintext
http://127.0.0.1:5000
```

If using the hardware stream, set the serial port before starting the backend:

```powershell
$env:SANJEEVANI_PORT="COM11"
$env:SANJEEVANI_BAUD="115200"
python dashboard/backend/server.py
```

If PowerShell blocks scripts, run this once in the same PowerShell window:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

### Telegram bot setup

Keep private values outside GitHub. Set them locally before running the backend:

```powershell
$env:TELEGRAM_BOT_TOKEN="your_private_bot_token"
$env:TELEGRAM_CHAT_ID="your_private_chat_id"
python dashboard/backend/server.py
```

Telegram commands:

```plaintext
/start
/status
/last
/emergencies
/resolve
/simulate normal
/simulate warning
/simulate emergency
/help
```

### Safety note

Do not upload bot tokens, chat IDs, Wi-Fi credentials, or private environment files to a public GitHub repository.

Sanjeevani AI is a research and demonstration prototype. It is not a certified clinical or medical device.

---

## Tech Stack

* **MYOSA Mini IoT Kit** for embedded sensing and physical response
* **ESP32 Arduino firmware** for sensor reading, filtering, feature extraction, OLED output, LED response, buzzer-ready response, and serial JSON stream
* **Python** for backend processing, simulation, event handling, and Telegram workflow
* **Flask** for REST API endpoints
* **Socket.IO** for real-time dashboard updates
* **SQLite** for local reading and emergency storage
* **HTML, CSS, and JavaScript** for the live command center dashboard
* **Telegram Bot API** for remote emergency communication
* **Synthetic sensor scenarios** for evaluation and demonstration

---

## Requirements / Installation

Install Python dependencies from the project root:

```bash
pip install flask flask-socketio pyserial requests python-dotenv
```

Recommended setup:

```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements_global.txt
```

For Arduino firmware, open the firmware sketch in Arduino IDE, select the correct ESP32 board and COM port, then upload the firmware to the MYOSA-connected ESP32 device.

---

## File Structure

```plaintext
sanjeevani-ai/
├── sanjeevani-ai.md
├── sanjeevani-ai-final-video.mp4
├── requirements_global.txt
├── start_final_windows.ps1
├── firmware/
│   └── main/
│       └── main.ino
├── ai-engine/
│   ├── calibration.py
│   ├── fall_detection.py
│   ├── feature_engineering.py
│   ├── risk_model.py
│   └── simulation.py
├── dashboard/
│   ├── backend/
│   │   ├── server.py
│   │   ├── serial_reader.py
│   │   ├── event_logger.py
│   │   └── db_init.py
│   ├── frontend/
│   │   ├── index.html
│   │   ├── style.css
│   │   └── app.js
│   └── database/
│       └── schema.sql
├── datasets/
│   └── synthetic_generator.py
├── testing/
│   ├── test_risk_engine.py
│   ├── test_fall_detection.py
│   ├── test_sensor_simulation.py
│   └── test_api.py
└── assets/
    └── images/
        └── sanjeevani_ai/
            ├── cover-dashboard.png
            ├── sensor-fusion-dashboard.png
            ├── myosa-hardware-stack.jpg
            ├── myosa-hardware-oled.jpg
            ├── myosa-hardware-angle.jpg
            ├── decision-matrix.png
            ├── environment-graph.png
            ├── motion-physiology-graph.png
            └── telegram-escalation.jpg
```

---

## License

This project is submitted for educational and innovation showcase purposes under the IEEE MYOSA Event 5.0 context.

All included dashboard screenshots and hardware photographs are original project materials from Team Sanjeevini AI.

---

## Contribution Notes

Future improvements may include multi-room monitoring, caregiver mobile views, cloud dashboards, smarter calibration, expanded dataset collection, machine-learning-assisted risk tuning, smart building integration, and structured real-world validation.

Any future contribution should preserve the core principle of Sanjeevani AI: explainable MYOSA sensor fusion for predictive emergency intelligence.