# Engineering-433MHz
This repository is about understanding how to use FS1000A/RF-5V 433,9 MHz sender/receivers and how to debug "malfunctioning" using ESP8266 and Arduino (see also https://lastminuteengineers.com/433mhz-rf-wireless-arduino-tutorial/) 

Wireless data transfer implies transforming data into radiowaves (https://en.wikipedia.org/wiki/Radio_frequency) 
and can be achieved in many ways amongst wich
-  BlueTooth
-  WIFI being commonly used in closed environments (e.g. workplace, airports, home) but for outside activities is not very much usable since it requires WIFI senders then connected to network typically through wires. It operates in the microwave range (1-6 GHz), and allows transfer rates up to 10 Gbit/second (https://en.wikipedia.org/wiki/Wi-Fi) .
- Radio transmission 433 MHz range 

# Hardware
- FS1000A 433,9 MHz emitter: XY-FST, 3  pins (VCC->5V, GND, DATA), operating mode AM, transfer rate 2400 bps, range 20-200m)
- RF-5V 433,9 MHz receiver, 4 pins (VCC->5V,  GND, DATA, DATA). It uses only 4mA, sensitivity -105 DB.
- Arduino Nano
- Arduino Mega 2560
- NodeMCU v3
- RTL-SDR 100kHz-1.7GHz Band FM Radio UV HF USB Tuner Receiver

# Software
- GQRX 2.11.5
- Audacity 2.3.3
- Arduino IDE 1.8.2

# Operating System
- macOS 10.15.4 (Catalina)

# Objective

Several tutorials are available that explain how RF works, and how to make it to work with Arduino. The above link for example shows also the theory of data modulation.
However, rarely there are tutorials about how to "debug" when the comunication does not work. Namely, when the message "Hello World" does not appear in the serial monitor of Arduino.

The purpose of this repository is to show a simple way to go through the whole chain and therefore also understand a bit better - hands on - how it all works together.

