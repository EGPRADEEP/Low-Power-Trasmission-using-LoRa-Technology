# 🚀 Interfacing LoRa SX1276 with STM32 (LR1276 915 MHz)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Author: EGPRADEEP](https://img.shields.io/badge/Author-EGPRADEEP-blue.svg)](https://github.com/EGPRADEEP)

This project demonstrates how to interface the **LoRa SX1276 (LR1276 915 MHz)** module with an **STM32F103C6T6 (Blue Pill)** microcontroller to wirelessly transmit temperature and humidity data (via DHT11) and display it on an OLED display.

---

## 📷 Project Preview

Sender and receiver modules connected on breadboards:

<p align="center">
  <img src="images/image0.jpg" alt="LoRa + STM32 setup" width="600"/>
</p>

Breadboard wiring close-up:

<p align="center">
  <img src="images/image1.jpg" alt="Connections close-up" width="600"/>
</p>

Circuit schematic:

<p align="center">
  <img src="images/image2.jpg" alt="Circuit diagram" width="600"/>
</p>

LoRa module wiring details:

<p align="center">
  <img src="images/image3.jpg" alt="LoRa module wiring" width="600"/>
</p>

---

## 📚 Table of Contents
- [Features](#-features)
- [Hardware Used](#-hardware-used)
- [Libraries](#-libraries)
- [Wiring & Schematics](#-wiring--schematics)
- [How It Works](#-how-it-works)
- [Folder Structure](#-folder-structure)
- [Installation & Usage](#-installation--usage)
- [Screenshots](#-screenshots)
- [License](#-license)
- [References](#-references)

---

## ✨ Features
- STM32 Blue Pill (STM32F103C6T6) microcontroller
- LoRa SX1276 LR1276‑915 MHz modules (sender + receiver)
- DHT11 temperature/humidity sensor
- I2C OLED display on receiver
- Built using STM32 HAL and LoRa_STM32 library

---

## 🔧 Hardware Used

| Component                       | Qty | Example Link |
|-------------------------------|-----|--------------|
| STM32F103 Blue Pill           | 2   | Local/E‑commerce |
| LoRa SX1276 (915 MHz)         | 2   | Local/E‑commerce |
| DHT11 Sensor                  | 1   | Local/E‑commerce |
| 0.96″ I2C OLED Display        | 1   | Local/E‑commerce |
| Jumper Wires, Breadboard, USB | —   | Local/E‑commerce |

---

## 📦 Libraries Used
- **LoRa_STM32** – SPI LoRa driver adapted for STM32 (based on Sandeep Mistry’s library)
- STM32 HAL (STM32CubeIDE-generated)
- Custom DHT and OLED HAL drivers

---

## 🔌 Wiring & Schematics

Refer to the images above. Detailed circuit diagrams and wiring steps are available in the original How2Electronics tutorial.

---

## ⚙️ How It Works
- **Sender:** Reads temperature/humidity via DHT11 and transmits via LoRa.
- **Receiver:** Receives LoRa packet and shows data on OLED display.

---

## 📁 Folder Structure

---

## ▶️ Installation & Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/EGPRADEEP/Interfacing-LoRa-SX1276-STM32.git
