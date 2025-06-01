Here’s a fresh, clean version of the `README.md` file for your **MiniFlightController\_v1 (DRACO\_MFC)** project:

---

````markdown
# 🚁 MiniFlightController_v1 (DRACO_MFC)

**MiniFlightController_v1**, also known as **DRACO_MFC**, is a compact and custom-designed 2-layer flight controller PCB based on the STM32F103C8Tx microcontroller. It is ideal for educational drone development, DIY UAVs, and embedded control systems.

---

## 🔧 Features

### 🧠 Microcontroller
- STM32F103C8Tx (ARM Cortex-M3, 72 MHz)
- USART-based bootloader
- External 8 MHz crystal oscillator
- Reset circuit with push-button

### 🔋 Power Supply
- XT60 / XT30 battery input (VIN, GND)
- SS14 diode for reverse protection
- AMS1117-3.3 linear regulator
- 10µF capacitors at input/output

### 🔄 ESC Interfaces
- 4 PWM outputs (PA1–PA4)
- 3-pin headers for ESC connection (VCC, GND, Signal)

### 📈 Sensors
- MPU6050 (I2C)
- Connected to PB6 (SCL), PB7 (SDA), INT to PA0

### 🔔 Status & Feedback
- RGB LED (power + activity indication)
- Driven via GPIOs (e.g., PA5, PA6)
- Buzzer circuit on PB0 (via NPN transistor + 1kΩ)

### 🔋 Battery Monitoring
- Voltage divider (2x 330Ω + 0.1µF cap)
- ADC input on PA7

### 🔌 I2C Expansion Header
- Exposes SDA, SCL, GND, VCC for future upgrades (barometer, compass, etc.)

### 💾 Programming Header
- 4-pin header: TX, RX, GND, VCC_3V3
- BOOT0 jumper and NRST pull-up

---

## 📐 Design Overview

- 📄 Schematic: Created in KiCad 7
- 🧩 PCB: 2-layer layout with optimized routing and minimal vias
- 🖨️ Mounting: 4 corner holes for M3 screws
- 📷 Silkscreen: Labeled pin headers, "DRACO_MFC v1.0", and author credits

---

## 📁 Folder Structure

```plaintext
MiniFlightController_v1/
├── KiCad/
│   ├── .sch  — Schematic file
│   ├── .kicad_pcb — PCB layout
│   └── .lib/.dcm — Custom libraries (if used)
├── Gerbers/ — Fabrication files
├── Images/  — 3D renders and top view
├── README.md
````

---

## ⚙️ Setup & Usage

1. Connect a LiPo battery (7–12V) to the power input.
2. Flash firmware using USB-TTL adapter (TX/RX → PA10/PA9).
3. Connect ESCs to the PWM outputs.
4. Monitor motion via MPU6050.
5. Use PA7 to read battery level in firmware.

---

## 🧪 Applications

* Quadcopter flight control
* Embedded robotics
* Sensor fusion experiments
* UAV prototype testing

---

## 📸 Previews

![3D Top View](./images/3d_top.png)
![Schematic Preview](./images/schematic_preview.png)

---

## 📜 License

MIT License
Designed by \[Your Name] | Version: DRACO\_MFC v1.0

---

## 🧠 Note

This board was made to balance simplicity, performance, and learning. It includes essential control and sensing while leaving room for future expansion and code flexibility.

```

---

Let me know if you'd like:
- A PDF export
- A GitHub-compatible `preview.gif`
- A cover image for LinkedIn or GitHub

Would you like help writing a LinkedIn post too?
```
