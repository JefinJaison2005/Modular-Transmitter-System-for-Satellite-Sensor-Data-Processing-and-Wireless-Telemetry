# Modular Transmitter System for Satellite Sensor Data Processing and Wireless Telemetry

A compact embedded telemetry system for real-time environmental sensing and long-range wireless transmission using LoRa.

---
Overview

This project implements a modular telemetry transmitter system that acquires environmental sensor data, processes it using a Teensy 4.1 microcontroller, and transmits it wirelessly using LoRa.

The system supports adaptive sampling, circular buffering, and structured telemetry packet transmission for reliable communication in satellite and IoT applications.

---

Features

* Multi-sensor data acquisition (UV, temperature, humidity, pressure, air quality)
* Adaptive sampling (dynamic rate adjustment)
* Circular buffer for efficient memory usage
* Structured telemetry packets with CRC error detection
* LoRa-based long-range communication (433 MHz)
* Store-and-forward transmission
* SDR-based signal verification

---

Hardware Used

* Teensy 4.1 Microcontroller
* GUVA-S12SD UV Sensor
* BME680 Environmental Sensor
* LoRa SX1278 Module
* DS3231 RTC Module
* 433 MHz Antenna

---

Software Used

* Arduino IDE
* Teensyduino
* Embedded C/C++
* LoRa Libraries
* Sensor Libraries
* SDR# (Signal Monitoring)

---

System Working

1. Sensor data is collected using ADC and I2C
2. Data is timestamped using RTC
3. Adaptive sampling adjusts data rate
4. Data is stored in a circular buffer
5. Telemetry packets are formed (Header + Seq + Time + Data + CRC)
6. Data is transmitted using LoRa
7. Signal is verified using SDR

---

Results

* Successful real-time sensor data acquisition
* Efficient adaptive sampling
* Reliable LoRa communication
* RF signal verified using RTL-SDR

---

Future Scope

* Ground station receiver implementation
* Data compression techniques
* Error correction (FEC)
* Low-power optimization
* Integration of additional sensors

---

Contributors

* Jefin Jaison – LoRa communication & telemetry
* Gouri Saji – Circular buffer & timestamping
* Nivedya Pavithran – Packet structure & CRC
* Thomas T Roy – Sensor interfacing & ADC

---
