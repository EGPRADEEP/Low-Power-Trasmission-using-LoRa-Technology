# 🚀 Interfacing LoRa SX1276 with STM32 (LR1276 915 MHz)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Author: EGPRADEEP](https://img.shields.io/badge/Author-EGPRADEEP-blue.svg)](https://github.com/EGPRADEEP)

This project demonstrates how to interface the **LoRa SX1276 (LR1276 915 MHz)** module with an **STM32F103C6T6 (Blue Pill)** microcontroller to wirelessly transmit data. It uses **SPI communication** and the **STM32 HAL library** to build a basic wireless system for long-range, low-power communication.

---

## 📸 Project Preview

<p align="center">
  <img src="images/image0.jpg" alt="LoRa STM32 Setup" width="600"/>
</p>

<p align="center">
  <img src="images/image1.jpg" alt="Breadboard Wiring" width="600"/>
</p>

---

## 📚 Table of Contents
- [✨ Features](#-features)
- [🔧 Hardware Used](#-hardware-used)
- [📦 Libraries](#-libraries)
- [🔌 Wiring & Schematics](#-wiring--schematics)
- [⚙️ How It Works](#-how-it-works)
- [📁 Folder Structure](#-folder-structure)
- [▶️ Installation & Usage](#-installation--usage)
- [🧪 Screenshots](#-screenshots)
- [📘 References](#-references)
- [🪪 License](#-license)

---

## ✨ Features
- LoRa SX1276 module communication at 915 MHz
- STM32F103C6T6 (Blue Pill) microcontroller
- SPI interface with STM32 HAL
- Serial output for debugging and logging
- Breadboard-friendly circuit for prototyping

---

## 🔧 Hardware Used

| Component                       | Qty |
|-------------------------------|-----|
| STM32F103C6T6 Blue Pill       | 2   |
| LoRa SX1276 (LR1276 915 MHz)  | 2   |
| FTDI or ST-LINK Programmer    | 2   |
| Breadboard + Jumper Wires     | –   |

---

## 📦 Libraries

- STM32 HAL (STM32CubeMX or Keil)
- [LoRa_STM32 Library](https://github.com/sandeepmistry/arduino-LoRa) (adapted)
- Custom SPI and UART configuration

---

## 🔌 Wiring & Schematics

### FTDI ↔ STM32 (for Serial Debugging)

---

## ⚙️ How It Works

1. LoRa modules initialized using STM32 HAL over SPI.
2. Frequency set to 915 MHz.
3. One board sends "Hello from STM32" repeatedly.
4. Other board receives and prints to Serial Monitor.
5. Communication confirmed through serial debug (115200 baud).

---

## 📁 Folder Structure

---

## ▶️ Installation & Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/EGPRADEEP/Interfacing-LoRa-SX1276-STM32.git
