# 🎶 Proximity Reactive System

A creative Arduino-based project developed during a hackathon, where distance becomes an interactive experience through light, sound, and motion.

## 🚀 Overview

This project uses an ultrasonic proximity sensor to detect distance and react dynamically through:

- 🎨 LED color feedback  
- 🌬️ Fan activation  
- 🎵 Sound output  

The system transforms distance into a multi-sensory interactive experience.

---

## ⚙️ How It Works

The ultrasonic sensor continuously measures distance:

- 🟢 **Object close** → Green LED  
- 🔴 **Object far away** → Red LED  
- 🌬️ Fan turns on when object is near  
- 🎶 Buzzer plays sound when proximity is detected  

---

## 🧩 Components

- Arduino Elegoo Uno (ATmega328P)
- Ultrasonic sensor (HC-SR04)
- LED + resistor
- Small DC fan
- Buzzer
- Transistor (for fan control)
- Breadboard and jumper wires

---

## 🔌 Pin Configuration

| Component            | Arduino Pin |
|----------------------|------------|
| Ultrasonic TRIG      | Digital 9  |
| Ultrasonic ECHO      | Digital 10 |
| LED                  | Digital 13 |
| Buzzer               | Digital 8  |
| Fan (via transistor) | Digital 6  |

> Note: The fan is controlled using a transistor to safely handle current.

---

## 🎯 Purpose

This project was created during a **hackathon** as a fun and creative experiment focused on:

- Interactive design  
- Sensor-based input  
- Real-time system response  

It is a **beginner-level project** aimed at learning through experimentation.

---

## 📦 Repository Contents

- `firmware/backup.hex` → Compiled Arduino firmware (Intel HEX format)

> ⚠️ The original `.ino` source code is not included.

---

## ⚡ Uploading the Firmware

To upload the firmware to an Arduino:
```bash
avrdude -c arduino -p atmega328p -P COM3 -b 115200 -U flash:w:backup.hex:i
```
Replace COM3 with your Arduino port.

---

## 👩‍💻 Authors

Pol Marcet (Destroyerrrocket on GitHub) & Claudia Córdoba

