Circuit diagram:-

1)
<img width="953" height="537" alt="image" src="https://github.com/user-attachments/assets/b61d53ae-dce1-4e28-ba08-a66645cfc4da" />


🛠️ ESP32 RTC Clock Display

📌 Overview

This project demonstrates how to connect an ESP32 with a DS1307 Real-Time Clock (RTC) and an I²C LCD Display. The ESP32 reads the date and time from the RTC and shows it on the LCD, making a simple digital clock.

✨ Features

Displays current Date (YYYY-MM-DD) and Time (HH:MM:SS)

Accurate timekeeping using DS1307 RTC

Programmed with MicroPython for simplicity

🔧 Hardware Required

ESP32 Development Board

DS1307 RTC Module with battery backup

I²C LCD Display (16x2 or 20x4 with PCF8574 adapter)

Jumper wires for connections

🔌 Wiring Connections

ESP32 GPIO21 (SDA) → SDA pins of RTC and LCD
ESP32 GPIO22 (SCL) → SCL pins of RTC and LCD
ESP32 VCC (3.3V or 5V) → VCC pins of RTC and LCD
ESP32 GND → GND pins of RTC and LCD

Note: Default I²C pins in the code are GPIO22 (SCL) and GPIO21 (SDA).

💻 Software Requirements

MicroPython firmware installed on ESP32

Required libraries: machine, SoftI2C, i2c_lcd.py, DS1307.py

🚀 Setup Instructions

Flash ESP32 with MicroPython.

Upload i2c_lcd.py and DS1307.py libraries to the ESP32.

Upload the main script (main.py).

Power the ESP32 → LCD will display the date and time.




##Circuit diagram:-

2)
<img width="735" height="462" alt="image" src="https://github.com/user-attachments/assets/222d8824-93a5-4d14-9ef3-fa70d978e27c" />

🌟 Project Name: ESP32 → DS1307 I²C Time Keeper ⏱️

💡 Overview

This project shows how to connect an ESP32 with a DS1307 Real-Time Clock (RTC) module using the I²C protocol. The ESP32 communicates with the DS1307 to read or set accurate date and time values. This is the essential base for building time-based applications such as clocks, loggers, or automation systems.

🔌 Wiring Guide

ESP32 GND → DS1307 GND

ESP32 3V3 or 5V → DS1307 VCC (depends on your RTC module)

ESP32 GPIO21 (SDA) → DS1307 SDA

ESP32 GPIO22 (SCL) → DS1307 SCL

Note: In the wiring image, the red wire powers the RTC from the ESP32’s 5V pin, while the black wire connects ground.

💻 Code Focus

The code (MicroPython or Arduino) does three main things:

Initializes the I²C bus on ESP32 pins GPIO21 (SDA) and GPIO22 (SCL).

Detects and accesses the DS1307 using its I²C address.

Reads the current time and date (and optionally sets it if required).

🚀 Use Cases

Displaying time on an LCD or OLED screen.

Timestamping data in logging systems.

Building real-time automation projects.
