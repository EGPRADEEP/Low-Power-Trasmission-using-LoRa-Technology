# 🚀 **Low-Power Long-Range Data Transmission Using LoRaWAN with STM32**



This project demonstrates a low-power wireless communication system using LoRaWAN (Long Range Wide Area Network) technology implemented on STM32F103C6T6 microcontrollers (Blue Pill) paired with SX1276 LoRa modules operating at 915 MHz. The system enables efficient point-to-point data transmission over long distances while consuming minimal energy, making it ideal for remote IoT applications, environmental monitoring, and telemetry systems.

📖 Project Overview
The project sets up a wireless communication link between two STM32 boards configured as transmitter (TX) and receiver (RX).The system is designed to simulate the key principles of LoRaWAN, focusing on:

Low power consumption
Long communication range

By utilizing the STM32 HAL library, this implementation offers modular firmware design and compatibility with various tools like AurduinoIDE.

🔧 Hardware Components
STM32F103C6T6 (Blue Pill) Microcontroller – 2 units

SX1276 LoRa Module (915 MHz) – 2 units

USB-to-Serial Adapter (ST-Link)

Breadboards and Jumper Wires

Power Supply (3.3V)

⚙️ How It Works
Transmitter Setup: The TX board reads a message or sensor value and sends it wirelessly using the SX1276 LoRa module via SPI.

Receiver Setup: The RX board receives the packet using its own SX1276 module and prints the data over UART to a serial monitor.

🧠 Use Cases
Remote Weather Stations

Smart Agriculture Monitoring

Disaster Area Communication Systems

▶️ How to Use
Clone the Repository:

git clone https://github.com/EGPRADEEP/Low-Power-Trasmission-using-LoRa-Technology.git

📚 References
LoRaWAN Overview – LoRa Alliance

SX1276 Datasheet – Semtech

STM32 HAL Documentation – STMicroelectronics

Original Project Inspiration – How2Electronics

📃 License
This project is licensed under the MIT License

Designed and developed with 💡 by EGPRADEEP

