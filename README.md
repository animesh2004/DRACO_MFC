# DRACO\_MFC - STM32-Based Mini Flight Controller

## 📦 Overview

DRACO\_MFC is a compact and powerful STM32F103C8Tx-based flight controller designed for small-scale drones and robotics projects. It integrates essential peripherals such as an MPU6050 sensor, ESC PWM outputs, status RGB LED, buzzer, and power management, all on a clean 2-layer PCB.

---

## 🔧 Features

* **STM32F103C8Tx** microcontroller (72 MHz, 64KB Flash)
* **MPU6050** IMU (Gyroscope + Accelerometer)
* **4 ESC PWM outputs** (PA1 to PA4)
* **USART Bootloader Interface** (PA9, PA10)
* **RGB Status LED** (PA5, PA6 + 3.3V)
* **Passive Buzzer** with NPN (PB0)
* **Battery Voltage Divider** (PA7)
* **SWD Debug Access** (PA13/PA14)
* **Reset + Boot Mode Buttons**
* **Power via XT60 or 2-pin header** (AMS1117 3.3V Regulated)

---

## 🖥️ Schematic Overview

All core modules are clearly modularized:

* Power Supply
* Microcontroller core
* Sensor interface
* ESC output zone
* Status indicators

---

## 📐 PCB Design

* **2-layer design** (Front/Back copper)
* Carefully routed analog + digital traces
* Decoupling capacitors near MCU and sensor
* Clear silkscreen labels for all headers

### 🧩 Connectors

| Header | Function        | Pins               |
| ------ | --------------- | ------------------ |
| J1     | Power Input     | VIN, GND           |
| J2     | Bootloader UART | TX, RX, VCC, GND   |
| J3–J6  | ESC Outputs     | PWM, VCC, GND      |
| J7     | I2C Breakout    | SDA, SCL, VCC, GND |

---

## 🚀 Getting Started

1. Power the board using XT60 or 2-pin header
2. Use USB-UART adapter on J2 to flash firmware
3. Use PA1–PA4 for ESC signal outputs
4. Connect MPU6050 directly or through I2C header

---

## 🧠 Future Improvements

* Add external flash or EEPROM
* Integrate GPS or barometer module
* Replace AMS1117 with buck converter for higher efficiency

---

## 🙌 Credits

* Designed using **KiCad 7.0**
* Inspired by open-source drone platforms

---

## 📬 Feedback?

Pull requests and suggestions are welcome. Feel free to fork and improve DRACO\_MFC!

> Designed with passion by \[Your Name] | v1.0 | 2025
