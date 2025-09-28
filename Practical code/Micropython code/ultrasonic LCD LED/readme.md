

# 📘 Ultrasonic Distance Measurement with ESP32, LCD & LED

## 🔹 Overview

This project uses an **ESP32**, an **HC-SR04 ultrasonic sensor**, an **I2C LCD**, and an **LED** to measure distance.

* The **ultrasonic sensor** detects distance.
* The **LCD** displays the measured distance.
* The **LED** blinks if the distance is **less than 40 cm**.

---

## 🔹 Components Required

* ESP32
* HC-SR04 Ultrasonic Sensor
* I2C LCD (16x2)
* LED + Resistor (220Ω recommended)
* Jumper wires & breadboard

---

## 🔹 Circuit Diagram
<img width="961" height="528" alt="image" src="https://github.com/user-attachments/assets/f7dfd5b7-15fb-40c5-bce8-2f0c780e91e8" />


Connections:

* **HC-SR04**:

  * VCC → 5V
  * GND → GND
  * TRIG → GPIO 5
  * ECHO → GPIO 18
* **I2C LCD**:

  * SDA → GPIO 21
  * SCL → GPIO 22
* **LED**:

  * Anode → GPIO 2
  * Cathode → GND

---

## 🔹 Steps

1. **Create New Project** on your ESP32 environment (Thonny, uPyCraft, or VS Code with MicroPython).
2. **Copy all library files** into your project folder:

   * `hcsr04.py` → Ultrasonic sensor library
   * `i2c_lcd.py` → LCD driver
   * `lcd_api.py` → LCD base API
   * `main.py` → Your main program logic

3. **Upload all files** to ESP32.
4. **Run `main.py`** → Distance prints on LCD, and LED blinks if distance < 50 cm.

---

## 🔹 Project Logic

* Ultrasonic sensor continuously measures distance.
* LCD shows `"Distance: XX.X cm"`.
* If distance `< 50 cm` → LED blinks on **GPIO 2**.
* Else LED stays **off**.



Would you like me to also **add screenshots of serial output + LCD output preview** into the `README.md` so it looks complete for GitHub?
