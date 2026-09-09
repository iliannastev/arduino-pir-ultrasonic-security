# Arduino Security System (PIR + Ultrasonic + IR Remote)

** Project – an alarm system with remote control and password access.**

## 📸 Video

## 🔧 How it works
- **PIR sensor** – detects motion (human body heat).
- **Ultrasonic sensor (HC‑SR04)** – measures distance and detects passing objects.
- The system is **armed/disarmed** via an **IR remote** with a 4‑digit code (`0000`).
- When motion or an object within 80 cm is detected, the **buzzer** sounds and the LCD shows which sensor triggered the alarm.

## ⚡ Hardware connections
| Component | Arduino Pin |
|-----------|-------------|
| LCD I2C SDA | A4 |
| LCD I2C SCL | A5 |
| Ultrasonic TRIG | 9 |
| Ultrasonic ECHO | 10 |
| Buzzer (+) | 11 |
| IR Receiver Signal | 12 |
| PIR Sensor OUT | 8 |

📸 * Schematics and block diagrams *

## 💻 Code
The code handles:
- Reading sensors and distance calculation.
- IR remote input and password verification.
- Alarm activation and system lock after 3 failed attempts.

📁 * Full code *

## 📦 Required Libraries (Arduino IDE)
- `LiquidCrystal_I2C` (by Frank de Brabander)
- `DIYables_IRcontroller` (by DIYables)

## 🎯 What I learned
- Integrating multiple sensors on one microcontroller.
- Difference between PIR (motion) and Ultrasonic (proximity) detection.
- Working with IR remote and password‑based security.
