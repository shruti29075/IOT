# ESP32 I2C LCD Counter with Backlight & LED

This project demonstrates how to use an **ESP32** with an **I2C 16x2 LCD** and an LED.  
The program:
- Displays "HELLO" on startup
- Counts from **1 to 10**
- Turns **LCD backlight + LED ON for odd numbers**
- Turns **LCD backlight + LED OFF for even numbers**
- Finally displays "Done Counting!"

---

## 🔌 Wiring (ESP32 → LCD 16x2 with I2C Backpack)
| ESP32 Pin | LCD Pin |
|-----------|---------|
| 3.3V      | VCC     |
| GND       | GND     |
| GPIO 21   | SDA     |
| GPIO 22   | SCL     |

LED is connected to **GPIO2** (onboard LED also works).

---

## ▶️ How to Run
1. Flash **MicroPython** firmware to ESP32.
2. Upload `main.py` and `i2c_lcd.py` to ESP32 using **Thonny / ampy / rshell**.
3. Reset ESP32 → LCD will display "HELLO" and start counting.

---

## 📦 Dependencies
- MicroPython
- `i2c_lcd.py` (HD44780 driver for I2C LCD)

