# 🚀 Low-Power LoRa Transmission with STM32 (915 MHz)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Author: EGPRADEEP](https://img.shields.io/badge/Author-EGPRADEEP-blue.svg)](https://github.com/EGPRADEEP)

A low-power, long-range wireless communication project demonstrating how to interface two **STM32F103C6T6 ("Blue Pill")** microcontrollers with **SX1276 LoRa modules** at 915 MHz using SPI and STM32 HAL. Transmit sensor or text data over several kilometers while minimizing energy consumption—ideal for remote IoT and telemetry systems.

---

## 📸 Project Preview

_Sender + Receiver breadboard setup and pin connections_

<p align="center">
  <img src="images/image0.jpg" alt="Setup view" width="600"/>
  <img src="images/image1.jpg" alt="Detailed wiring TX" width="600"/>
  <img src="images/image2.jpg" alt="Detailed wiring RX" width="600"/>
  <img src="images/image3.jpg" alt="Serial monitor output" width="600"/>
</p>

---

## 📚 Table of Contents
- [✨ Features](#-features)
- [🔧 Hardware Used](#-hardware-used)
- [📦 Software & Libraries](#-software--libraries)
- [🔌 Wiring & Schematics](#-wiring--schematics)
- [⚙️ How It Works](#️-how-it-works)
- [📁 Folder Structure](#-folder-structure)
- [▶️ Installation & Usage](#️-installation--usage)
- [🧪 Testing & Output](#-testing--output)
- [🔗 References](#-references)
- [📃 License](#-license)

---

## ✨ Features

- Ultra-low power consumption via sleep mode between LoRa transmissions  
- Simple point-to-point communication using SX1276 (915 MHz) over SPI  
- STM32Blue Pill microcontroller and HAL library firmware  
- Console output via UART (115200 baud) for easy debugging  
- Modular architecture: setup as TX or RX using a single codebase  

---

## 🔧 Hardware Used

| Hardware                        | Quantity |
|-------------------------------|----------|
| STM32F103C6T6 Blue Pill       | 2        |
| SX1276 LoRa Module (915 MHz) | 2        |
| FTDI USB‑Serial Adapter       | 1–2      |
| Jumper wires & Breadboards    | —        |

---

## 📦 Software & Libraries

- STM32 HAL drivers (generated via CubeMX or Keil)  
- SX1276 LoRa driver (adapted for STM32)  
- Optional enhancements: integrate sensors (e.g., DHT11) or display modules (e.g., OLED)

---

## 🔌 Wiring & Schematics

### FTDI ↔ STM32 (UART)

---

## ⚙️ How It Works

1. Choose mode in `main.c`:  
   ```c
   #define TX  // Sender mode
   //#define RX // Receiver mode
🔗 References
SX1276 datasheet (Semtech)

STM32 LoRa driver adaptation (e.g., domski.pl blog)

📃 License
This project is distributed under the MIT License.

Made by EGPRADEEP
