# Fire-Fighting-Robot

# 🔥 Fire Fighting Robot (ESP8266 + Blynk)

A DIY IoT-based fire fighting robot that can be remotely controlled via the Blynk app.  
Built with ESP8266, flame sensor, relay‑driven water pump, and motor driver for directional control.

---

## 🚀 Features
- Remote control (forward, backward, left, right) via Blynk app buttons
- Real‑time flame detection displayed on Blynk dashboard
- Automatic activation of water pump when flame is detected
- Manual pump control from app
- Status feedback via Serial Monitor

---

## ⚙️ Hardware Used
- ESP8266 NodeMCU board
- Motor driver (L298N or equivalent)
- Flame sensor
- Relay module + water pump motor
- 4 DC motors & chassis
- Blynk IoT app

---

## 📦 Software & Libraries
- Arduino IDE
- Blynk Library
- ESP8266WiFi
- BlynkSimpleEsp8266

---

## 🧰 Pin Configuration
| Function          | Pin |
|------------------:|:--:|
| Motor IN1         | D1 |
| Motor IN2         | D2 |
| Motor IN3         | D3 |
| Motor IN4         | D4 |
| Relay (Pump)      | D6 |
| Flame Sensor Out  | D7 |

*(ENA/ENB are commented out in code; adjust based on motor driver used)*

---

## 📲 Blynk Virtual Pins
| Pin  | Function             |
|----:|---------------------:|
| V0  | Forward Button        |
| V1  | Backward Button       |
| V2  | Left Button           |
| V3  | Right Button          |
| V5  | Manual Pump Control   |
| V6  | Flame sensor status   |

---

## 🧪 How It Works
- Robot receives movement commands from Blynk app
- Flame sensor detects fire → status sent to Blynk (V6)
- Relay is activated automatically or manually to spray water
- Real‑time monitoring via Blynk dashboard & Serial output
