# ESP32 Ultrasonic Sensor with LED (Wokwi Simulation)

This project demonstrates how to use an **ESP32** with an **HC-SR04 Ultrasonic Sensor** and an **LED** in MicroPython.

## 🚀 Features
- Measures distance using the ultrasonic sensor.
- Turns **LED ON if object is closer than 50 cm**, otherwise LED remains OFF.
- Runs in **Wokwi Simulator** or on real ESP32 hardware.

## 🔌 Wiring (ESP32 → HC-SR04 + LED)
| ESP32 Pin | HC-SR04 Pin |
|-----------|-------------|
| 3.3V      | VCC         |
| GND       | GND         |
| GPIO 21   | Trig        |
| GPIO 22   | Echo        |

| ESP32 Pin | LED Pin |
|-----------|---------|
| GPIO 26   | Anode (+) |
| GND       | Cathode (-) |

⚠️ Note: On real hardware, HC-SR04 works at **5V**. Use a **voltage divider or level shifter** on the Echo pin.

## ▶️ How to Run
1. Flash **MicroPython** to ESP32.
2. Upload `main.py` and `hcsr04.py` to the board.
3. Run in **Wokwi** with the provided `diagram.json`.

## 📦 Dependencies
- MicroPython
- `hcsr04.py` driver
