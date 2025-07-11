# Low-Power-Trasmission-using-LoRa-Technology

# 🚀 Interfacing LoRa SX1276 with STM32 Microcontroller (LR1276 915MHz)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Made with Love](https://img.shields.io/badge/Made%20with-Love-red.svg)](https://github.com/EGPRADEEP)

This project demonstrates how to interface the **LoRa SX1276 (LR1276-915MHz) module** with an **STM32F103C6T6** microcontroller using the **LoRa_STM32** library. The goal is to transmit temperature and humidity sensor data wirelessly via LoRa.

> 📡 Ideal for low-power, long-range communication projects using STM32 and LoRa.

---

## 📷 Project Preview

<p align="center">
  <img src="images/stm32-lora-setup.jpg" alt="STM32 LoRa Setup" width="600"/>
</p>

---

## 📚 Table of Contents
- [Features](#-features)
- [Hardware Used](#-hardware-used)
- [Library Used](#-library-used)
- [Wiring Diagram](#-wiring-diagram)
- [How It Works](#-how-it-works)
- [Folder Structure](#-folder-structure)
- [How to Run](#-how-to-run)
- [Screenshots](#-screenshots)
- [License](#-license)
- [References](#-references)

---

## ✨ Features

- STM32F103C6T6T6 (Blue Pill) microcontroller
- LoRa communication via SX1276 LR1276-915MHz module
- DHT11 temperature and humidity sensor
- OLED display on the receiver side
- Wireless data transfer over 915 MHz
- STM32 HAL and LoRa_STM32 library based implementation

---

## 🔧 Hardware Used

| Component                          | Quantity | Buy Link |
|-----------------------------------|----------|----------|
| STM32F103C6T6 Blue Pill           | 2        | [Amazon](https://amzn.to/3sZvAx9) |
| LoRa SX1276 (LR1276 915 MHz)      | 2        | [Amazon](https://amzn.to/3rW2YBA) |
| DHT11 Sensor                      | 1        | [Amazon](https://amzn.to/3sZDg6j) |
| 0.96" I2C OLED Display            | 1        | [Amazon](https://amzn.to/3yq0ZUB) |
| Jumper Wires, Breadboard, USB Cable | —      | Local/E-commerce |

---

## 📦 Library Used

- [LoRa_STM32](https://github.com/sandeepmistry/LoRa) – A LoRa communication library ported for STM32
- STM32 HAL Drivers (via STM32CubeIDE)
- DHT HAL driver (custom implementation)

---

## 🔌 Wiring Diagram

<p align="center">
  <img src="images/stm32-lora-circuit.jpg" alt="Circuit Diagram" width="600"/>
</p>

See full schematic at [How2Electronics Article](https://how2electronics.com/interfacing-lora-sx1276-with-stm32-microcontroller-lr1276-915mhz/)

---

## ⚙️ How It Works

- **Sender Side:** Reads temperature and humidity from the DHT11 sensor and transmits the values via the LoRa module.
- **Receiver Side:** Receives LoRa packets and displays the data on a 0.96" OLED I2C screen.

---

## 📁 Folder Structure

---

## ▶️ How to Run

### Prerequisites:
- STM32CubeIDE installed
- USB-TTL for uploading if needed
- I2C and UART peripherals configured in `.ioc` file

### Steps:
1. Clone the repo  
   ```bash
   git clone https://github.com/EGPRADEEP/Interfacing-LoRa-SX1276-STM32.git

---

## ✅ Next Steps for You

1. Upload the images (`stm32-lora-setup.jpg`, `stm32-lora-circuit.jpg`, `output-screenshot.png`) into a folder named `/images` in your repo.
2. Create a `LICENSE` file with [MIT License](https://choosealicense.com/licenses/mit/).
3. Paste the above content into your `README.md`.
4. Push your changes using:
   ```bash
   git add .
   git commit -m "Add professional README and images"
   git push origin main

