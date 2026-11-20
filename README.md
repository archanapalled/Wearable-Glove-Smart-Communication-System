# Wearable Smart Gloves Communication System

## 📌 Project Overview

The Wearable Smart Gloves Communication System is an assistive technology project designed to help people with speech and communication difficulties communicate through hand gestures.

The system uses flex sensors attached to a glove to detect finger movements. An Arduino Nano processes the sensor values and identifies predefined gestures. Corresponding messages are displayed on a 16x2 LCD.

## 🎯 Project Objective

To develop a wearable communication system that converts predefined hand gestures into readable messages, helping improve communication accessibility.

## ✨ Features

### Gesture Detection
- Uses four flex sensors to detect finger movements.
- Reads sensor values through Arduino analog input pins.
- Identifies predefined gestures using threshold conditions.

### Message Display
- Displays corresponding messages on a 16x2 LCD.
- Shows detected gestures such as:
  - WASHROOM
  - DRINK WATER
  - FOOD
  - FRUIT
  - NOTHING

### LED Indication
- Uses an LED to indicate selected gesture conditions.

### Serial Monitoring
- Displays sensor readings through the Arduino Serial Monitor.
- Helps observe sensor values and understand gesture detection.

## 🏗️ Technology Stack

| Category | Technologies |
|---|---|
| Microcontroller | Arduino Nano |
| Programming | Arduino C/C++ |
| Sensors | Flex Sensors |
| Display | 16x2 LCD with I2C Module |
| Output | LED |
| Communication | Serial Monitor |
| Development Environment | Arduino IDE |

## 🔧 Hardware Components

- Arduino Nano
- Four Flex Sensors
- 16x2 LCD Display
- I2C Module
- LED
- Connecting Wires
- Glove
- DFPlayer Mini, SD Card and Speaker (planned audio extension)

## ⚙️ Working Principle

1. Flex sensors detect bending movements of the fingers.
2. Arduino Nano reads the analog values from four sensors.
3. The program compares sensor readings with predefined threshold values.
4. Based on the detected gesture, the corresponding message is selected.
5. The message is displayed on the LCD.
6. The LED indicates selected gesture conditions.

## 🔌 Pin Configuration

| Component | Arduino Pin |
|---|---|
| Flex Sensor 1 | A0 |
| Flex Sensor 2 | A1 |
| Flex Sensor 3 | A2 |
| Flex Sensor 4 | A3 |
| LED | Digital Pin 13 |
| LCD SDA | A4 (Arduino Nano) |
| LCD SCL | A5 (Arduino Nano) |

## 💻 Software Requirements

- Arduino IDE
- Arduino AVR Boards package
- Wire Library
- LiquidCrystal_I2C Library

## 🚀 Getting Started

### Step 1: Install Arduino IDE

Download and install Arduino IDE.

### Step 2: Install Required Library

1. Open Arduino IDE.
2. Navigate to Sketch → Include Library → Manage Libraries.
3. Search for LiquidCrystal I2C.
4. Install a compatible library.

### Step 3: Open the Project

1. Download or clone this repository.
2. Open the `.ino` file in Arduino IDE.
3. Select Arduino Nano under Tools → Board.

### Step 4: Configure the Board

- Select the appropriate COM port.
- Verify the code.
- Upload the sketch to Arduino Nano.

### Step 5: Monitor Output

Open Serial Monitor and set the baud rate to 9600 to observe sensor readings and detected messages.

## 📊 Gesture Mapping

| Sensor | Detected Message |
|---|---|
| Flex Sensor 1 (A0) | WASHROOM |
| Flex Sensor 2 (A1) | DRINK WATER |
| Flex Sensor 3 (A2) | FOOD |
| Flex Sensor 4 (A3) | FRUIT |
| No detected gesture | NOTHING |

## 🎯 Applications

- Assistive communication technology
- Gesture-based communication systems
- Embedded systems learning
- Sensor-based automation projects
- Human-computer interaction

## 🔮 Future Enhancements

- Integrate DFPlayer Mini for voice output.
- Add speaker-based audio messages.
- Improve gesture recognition accuracy.
- Support additional hand gestures.
- Develop a more compact and comfortable wearable design.

## 📝 Project Status

Arduino code compilation completed successfully.

Physical hardware testing and sensor calibration are pending.

Audio playback using DFPlayer Mini is planned as a future enhancement.

## 👩‍💻 Developed Using

Arduino Nano | Flex Sensors | Arduino IDE | Embedded C/C++
