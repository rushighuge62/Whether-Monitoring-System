# IoT Based Weather Monitoring System using NodeMCU and ThingSpeak

## 📦 Overview

This project implements an IoT-based weather monitoring system using NodeMCU (ESP8266) and the ThingSpeak platform. It allows for real-time monitoring of temperature, humidity, and other environmental parameters remotely. The data collected is transmitted to ThingSpeak, where it can be visualized, analyzed, and logged for further processing.

## ✅ Features

* **Real-time Data Monitoring:** Continuously monitors temperature and humidity.
* **Web-Based Dashboard:** Data visualization on the ThingSpeak platform.
* **Data Logging:** Stores historical data for trend analysis.
* **Alert System:** Configurable alerts based on predefined environmental thresholds.

## 🛠️ Components and Hardware

* NodeMCU ESP8266
* DHT11 Temperature and Humidity Sensor
* USB Cable
* Breadboard and Jumper Wires
* Power Supply

## 📋 Prerequisites

* Arduino IDE
* ThingSpeak Account
* Libraries:

  * `ESP8266WiFi.h`
  * `DHT.h`

## 🔧 Circuit Diagram
Connect the pins according to following pairs below: 
```
   +----------------------------------+
   |        NodeMCU (ESP8266)         |
   |                                  |
   |  D0 (GPIO 16) --> DHT11 Data Pin |
   |  3V3         --> DHT11 VCC       |
   |  GND         --> DHT11 GND       |
   +----------------------------------+
```

## 🚀 Getting Started

### 1. Hardware Setup

* Connect the DHT11 sensor to NodeMCU as per the circuit diagram.
* Ensure stable power supply and reliable WiFi connection.

### 2. Software Setup

* Open the Arduino IDE and install the required libraries:

  * `DHT sensor library`
  * `ESP8266WiFi library`

* Update the sketch with your WiFi credentials and ThingSpeak API keys.

### 3. ThingSpeak Setup

* Create a new channel on ThingSpeak.
* Add fields for Temperature and Humidity.
* Copy the Write API Key for later use.

### 4. Upload the Sketch

* Connect NodeMCU to your computer via USB.
* Select the correct COM port and board type in the Arduino IDE.
* Upload the code (code.c file) and open the Serial Monitor to confirm data transmission.

## 📊 Data Visualization

* Access your ThingSpeak channel to view the real-time data feed.
* Utilize ThingSpeak’s built-in data analysis and visualization tools.

## 🚨 Alerts and Notifications

* Configure alerts within ThingSpeak based on data thresholds.
* Implement SMS or Email alerts using ThingSpeak plugins.

## 🔄 Troubleshooting

* Ensure NodeMCU is properly connected to WiFi.
* Verify API key and channel ID in the code.
* Check sensor connections and power supply.

## 📝 Additional Information

* Adjust data logging intervals as per project requirements.
* Optimize power usage for battery-operated deployments.

