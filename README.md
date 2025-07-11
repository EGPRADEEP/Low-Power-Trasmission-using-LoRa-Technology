# 🚀 Interfacing LoRa SX1276 with STM32 (LR1276 915 MHz)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Author: EGPRADEEP](https://img.shields.io/badge/Author-EGPRADEEP-blue.svg)](https://github.com/EGPRADEEP)

This project demonstrates how to interface the **LoRa SX1276 (LR1276 915 MHz)** module with an **STM32F103C6T6 (Blue Pill)** microcontroller using SPI to establish long-range, low-power wireless communication. It sends data from a transmitter STM32 to a receiver STM32 board via LoRa and displays output using UART or optionally on an OLED display.

The project is ideal for **IoT communication**, **remote sensor networks**, and **embedded wireless systems** development.

---

## 📷 Project Preview

Sender and receiver on breadboards:

<p align="center">
  <img src="images/image0.jpg" alt="LoRa + STM32 setup" width="600"/>
</p>

LoRa TX module wiring:

<p align="center">
  <img src="images/image1.jpg" alt="TX Wiring" width="600"/>
</p>

LoRa RX module wiring:

<p align="center">
  <img src="images/image2.jpg" alt="RX Wiring" width="600"/>
</p>

Serial output from receiver:

<p align="center">
  <img src="images/image3.jpg" alt="Serial Monitor Output" width="600"/>
</p>

---

## 📚 Table of Contents
- [✨ Features](#-features)
- [🔧 Hardware Used](#-hardware-used)
- [📦 Libraries Used](#-libraries-used)
- [🔌 Wiring & Schematics](#-wiring--schematics)
- [⚙️ How It Works](#️-how-it-works)
- [📁 Folder Structure](#-folder-structure)
- [▶️ Installation & Usage](#️-installation--usage)
- [🧪 Testing & Output](#-testing--output)
- [🔗 References](#-references)
- [📃 License](#-license)

---

## ✨ Features

- Long-range wireless data transfer using LoRa SX1276 (915 MHz)
- STM32F103C6T6 (Blue Pill) microcontroller-based implementation
- SPI-based communication using STM32 HAL libraries
- Serial debugging output for data transmission verification
- Easy expansion for DHT11 sensor or OLED integration

---

## 🔧 Hardware Used

| Component                       | Quantity |
|-------------------------------|----------|
| STM32F103C6T6 Blue Pill       | 2        |
| LoRa SX1276 (915 MHz) Module  | 2        |
| FTDI USB to Serial Adapter    | 1–2      |
| Jumper Wires                  | As needed |
| Breadboards                   | 2        |

---

## 📦 Libraries Used

- **LoRa_STM32** – Adapted LoRa driver for STM32 (based on Sandeep Mistry’s Arduino LoRa library)
- **STM32 HAL** – Hardware Abstraction Layer generated via STM32CubeMX or Keil
- (Optional) DHT and OLED drivers for sensor/display use

---

## 🔌 Wiring & Schematics


---

## ⚙️ How It Works

1. **TX board** sends hardcoded or sensor-acquired data via LoRa.
2. **RX board** receives packets and logs them via UART.
3. LoRa configured for **915 MHz**, using SPI and HAL.
4. UART output shown on serial monitor (e.g., Tera Term @115200 baud).

You can enable either transmitter or receiver code in `main.c`:

▶️ Installation & Usage
Clone the repo:
git clone https://github.com/EGPRADEEP/LoRa-SX1276-STM32.git
🔗 References
📘 How2Electronics Project Tutorial

📘 Semtech SX1276 Datasheet

📘 STM32 HAL LoRa Driver (W. Domski)

📃 License
This project is licensed under the MIT License.

Designed by EGPRADEEP

