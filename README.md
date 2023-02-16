# README

Author(s): Sam Kovnar

## About this repository

This repository contains the code used to test the Communications
subsystem of the Wherehouse, Team 23's Spring 2023 ECE senior design
project.

## Setup and Requirements

This code has been tested on Ai-Thinker's ESP8266 ESP-01 modules.
It had been built and tested using the Arduino IDE.

### Software dependencies

Arduino IDE v2.0.0 or later

ESP8266 Core for Arduino
- ESP8266WiFi.h
- ESP8266HTTPClient.h
- ESP8266WiFiMulti.h

WiFiClient.h

ESPAsyncWebServer.h

## Tested Software Versions

Operating System >>> Ubuntu 22.04 LTS
Arduino IDE >>> v2.0.3

## Repository Contents

### Arduino Code

esp8266_ap_test         -> Code for ESP8266 acting as Access Point
esp8266_sta_test        -> Code for ESP8266 acting as Station

The above two code files are a simple test of the ESP8266 WiFi libraries.
The Access Point device should produce serial output that a WiFi access point
was started successfully. Once the Access Point is created, the Station device
should be able to connect and display connection status over Serial lines.

This code was last tested 2023-02-14.

esp8266_ap_http_test    -> Code for ESP8266 acting as Access Point
esp8266_sta_http_test   -> Code for ESP8266 acting as Station

The above two code files are based on a tutorial by RandomNerdTutorials
at https://randomnerdtutorials.com/esp8266-nodemcu-client-server-wi-fi/.
Each should be loaded onto an ESP8266. When both ESP devices are active
(i.e. powered on and running in operation mode), the Station device should
be able to receive data from the Access Point device by requesting from
the /data URL.

This code was last tested 2023-02-16.

