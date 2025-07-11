##🚀 Low-Power Long-Range Data Transmission Using LoRaWAN with STM32



This project demonstrates a low-power wireless communication system using LoRaWAN (Long Range Wide Area Network) technology implemented on STM32F103C6T6 microcontrollers (Blue Pill) paired with SX1276 LoRa modules operating at 915 MHz. The system enables efficient point-to-point data transmission over long distances while consuming minimal energy, making it ideal for remote IoT applications, environmental monitoring, and telemetry systems.

📖 Project Overview
The project sets up a wireless communication link between two STM32 boards configured as transmitter (TX) and receiver (RX). Data packets are transmitted using the LoRa PHY layer, and the system is designed to simulate the key principles of LoRaWAN, focusing on:

Low power consumption

Long communication range

High signal penetration

Simple architecture for embedded development

By utilizing the STM32 HAL library, this implementation offers modular firmware design and compatibility with various embedded development tools like Keil uVision and STM32CubeIDE.

✨ Key Features
Ultra Low-Power Operation: Sleep mode enabled between transmissions

Long-Range Communication: 915 MHz LoRa modulation for extended range

STM32-Based Design: Efficient ARM Cortex-M3 processing using HAL

Flexible Deployment: Easy switching between TX and RX roles

UART Monitoring: Serial output for real-time data visualization

Extendable Architecture: Integration with sensors (e.g., DHT11) or displays (e.g., OLED) supported

🔧 Hardware Components
STM32F103C6T6 (Blue Pill) Microcontroller – 2 units

SX1276 LoRa Module (915 MHz) – 2 units

USB-to-Serial Adapter (ST-Link)

Breadboards and Jumper Wires

Power Supply (3.3V)

⚙️ How It Works
Transmitter Setup: The TX board reads a message or sensor value and sends it wirelessly using the SX1276 LoRa module via SPI.

Receiver Setup: The RX board receives the packet using its own SX1276 module and prints the data over UART to a serial monitor.

Power Optimization: Between transmissions, the microcontroller and radio module can be put into low-power or sleep mode to reduce energy usage.

Protocol Configuration: Although LoRaWAN requires a network stack and gateways, this project emulates the LoRa physical layer of LoRaWAN for simplicity and learning purposes.

🧠 Use Cases
Remote Weather Stations

Smart Agriculture Monitoring

Asset and Wildlife Tracking

Disaster Area Communication Systems

Battery-Operated Sensor Nodes

📁 Project Structure
css
Copy
Edit
/
├── Core/                 → STM32 HAL code (Drivers + App)
├── Drivers/              → SX1276 LoRa driver
├── main.c                → Core logic for TX/RX
├── LowPowerLoRa.uvprojx  → Keil project file
├── README.md
└── LICENSE
▶️ How to Use
Clone the Repository:

bash
Copy
Edit
git clone https://github.com/EGPRADEEP/Low-Power-Trasmission-using-LoRa-Technology.git
Open in Keil uVision or STM32CubeIDE

Select Role in Code:
In main.c, uncomment the appropriate mode:

c
Copy
Edit
#define TX  // for transmitter
//#define RX // for receiver
Flash the Code to your STM32 boards (TX & RX)

Monitor Output using any UART serial terminal at 115200 baud

📚 References
LoRaWAN Overview – LoRa Alliance

SX1276 Datasheet – Semtech

STM32 HAL Documentation – STMicroelectronics

Original Project Inspiration – How2Electronics

📃 License
This project is licensed under the MIT License

Designed and developed with 💡 by EGPRADEEP

