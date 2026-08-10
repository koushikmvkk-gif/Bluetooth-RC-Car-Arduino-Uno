# 🚗 Bluetooth Controlled RC Car using Arduino Uno

<div align="center">

![Arduino](https://img.shields.io/badge/Arduino-UNO-blue.svg)
![Bluetooth](https://img.shields.io/badge/Bluetooth-HC--05%20%7C%20HC--06-green.svg)
![Motor Driver](https://img.shields.io/badge/Motor%20Driver-L298N-red.svg)
![Language](https://img.shields.io/badge/Language-C%2FC%2B%2B-orange.svg)
![Platform](https://img.shields.io/badge/Platform-Arduino_IDE-lightgrey.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

**A Smartphone Controlled Bluetooth RC Car using Arduino Uno**

Control a four-wheel robotic vehicle wirelessly using an Android smartphone via Bluetooth communication. The robot can move forward, backward, left, right, and stop using simple Bluetooth commands sent from any compatible Bluetooth controller application.

</div>

---

# 📖 Overview

The **Bluetooth RC Car** is an Arduino-based wireless robotic vehicle that receives commands from a smartphone through an HC-05/HC-06 Bluetooth module. The Arduino processes the incoming serial commands and controls the DC motors using an L298N Motor Driver.

This project is an excellent beginner-to-intermediate robotics project that introduces:

- Arduino Programming
- Bluetooth Communication
- Mobile Robot Control
- Motor Driver Interfacing
- Wireless Embedded Systems
- Differential Drive Robotics

---

# ✨ Features

- 📱 Wireless Bluetooth Control
- 🚗 Forward Movement
- 🔄 Backward Movement
- ⬅ Left Turn
- ➡ Right Turn
- 🛑 Instant Stop
- ⚡ Real-Time Response
- 🔋 Battery Powered
- 📡 10–15 Meter Bluetooth Range
- 🔧 Easy to Modify
- 🤖 Four Wheel Differential Drive
- 📲 Compatible with Android Bluetooth Controller Apps

---

# 🛠 Hardware Requirements

| Component | Quantity |
|-----------|----------|
| Arduino Uno | 1 |
| HC-05 / HC-06 Bluetooth Module | 1 |
| L298N Motor Driver Module | 1 |
| BO DC Motors | 4 |
| Robot Chassis | 1 |
| Wheels | 4 |
| Castor Wheel (Optional) | 1 |
| 18650 Battery Pack / 7.4V Li-ion Battery | 1 |
| Battery Holder | 1 |
| Power Switch | 1 |
| Jumper Wires | As Required |
| Breadboard (Optional) | 1 |

---

# 🔌 System Architecture

```
Android Phone
        │
 Bluetooth Commands
        │
     HC-05 Module
        │
Serial Communication
        │
   Arduino UNO
        │
Motor Control Logic
        │
     L298N Driver
        │
 ┌───────────────┐
 │               │
Left Motors   Right Motors
 │               │
Robot Movement
```

---

# ⚙ Working Principle

1. User pairs the smartphone with the HC-05 Bluetooth module.
2. A Bluetooth controller app sends movement commands.
3. HC-05 receives the commands.
4. Arduino reads the serial data.
5. Arduino interprets the command.
6. Corresponding motor driver pins are activated.
7. L298N powers the motors.
8. The RC car moves according to the received command.

---

# 📲 Bluetooth Commands

| Command | Action |
|----------|--------|
| F | Move Forward |
| B | Move Backward |
| L | Turn Left |
| R | Turn Right |
| S | Stop |

Additional commands can be programmed for speed control or custom movements.

---

# 🔌 Circuit Connections

## HC-05 Bluetooth Module

| HC-05 | Arduino Uno |
|--------|-------------|
| VCC | 5V |
| GND | GND |
| TX | RX (Pin 0) |
| RX | TX (Pin 1) *(Use Voltage Divider Recommended)* |

---

## L298N Motor Driver

| L298N | Arduino |
|--------|----------|
| IN1 | D8 |
| IN2 | D9 |
| IN3 | D10 |
| IN4 | D11 |
| ENA | D5 (PWM) |
| ENB | D6 (PWM) |
| GND | GND |
| 12V | Battery Positive |

---

## Motors

| Motor | Connection |
|--------|------------|
| Left Motors | OUT1 & OUT2 |
| Right Motors | OUT3 & OUT4 |

---

# 📂 Project Structure

```
Bluetooth-RC-Car-Arduino-Uno/
│
├── Arduino_Code/
│   └── Bluetooth_RC_Car.ino
│
├── Circuit_Diagram/
│   └── Bluetooth_RC_Car_Circuit.png
│
├── Images/
│   ├── Robot.jpg
│   ├── Chassis.jpg
│   ├── Wiring.jpg
│   └── App.jpg
│
├── Videos/
│   └── Demo.mp4
│
├── Documentation/
│   └── Project_Report.pdf
│
├── LICENSE
└── README.md
```

---

# 💻 Software Requirements

- Arduino IDE
- Bluetooth Controller App
- USB Driver for Arduino Uno

---

# 📱 Recommended Android Apps

- Arduino Bluetooth Controller
- Bluetooth RC Controller
- Bluetooth Electronics
- Serial Bluetooth Terminal
- Bluetooth Terminal HC-05

---

# 🚀 Installation

## Step 1

Clone the repository.

```bash
git clone https://github.com/yourusername/Bluetooth-RC-Car-Arduino-Uno.git
```

---

## Step 2

Open the Arduino sketch.

```
Bluetooth_RC_Car.ino
```

---

## Step 3

Install the required libraries (if applicable).

---

## Step 4

Select:

- Board → Arduino Uno
- Correct COM Port

---

## Step 5

Upload the program.

---

## Step 6

Disconnect USB.

---

## Step 7

Power the robot using the battery.

---

## Step 8

Pair your smartphone with HC-05.

Default Password:

```
1234
```

or

```
0000
```

---

## Step 9

Open the Bluetooth Controller App.

---

## Step 10

Connect and start driving the robot.

---

# 🎮 Robot Controls

| Button | Robot Action |
|----------|-------------|
| ↑ | Forward |
| ↓ | Backward |
| ← | Left |
| → | Right |
| ■ | Stop |

---

# 🔋 Power Supply

Recommended:

- 2 × 18650 Li-ion Battery (7.4V)
- 7.4V LiPo Battery
- 9V Rechargeable Battery (Light Load Only)

Arduino can be powered using:

- VIN Pin
- DC Jack

Motor Driver receives battery supply directly.

---

# 📊 Applications

- Robotics Learning
- STEM Education
- College Mini Projects
- Wireless Robot Platform
- Home Automation Base Robot
- Obstacle Avoidance Base Platform
- Line Following Robot Upgrade
- Surveillance Robot Prototype
- Research Projects
- Embedded Systems Practice

---

# 📈 Future Improvements

- 📷 ESP32-CAM Live Video Streaming
- 🌐 WiFi Control
- 🎮 Joystick Mobile Interface
- 🎤 Voice Control
- 🤖 Autonomous Navigation
- 📍 GPS Tracking
- 📡 IoT Integration
- ☁ Cloud Monitoring
- 🔋 Battery Level Monitoring
- 🚧 Obstacle Avoidance
- 📱 Custom Android Application
- ⚡ Speed Control using PWM
- 🧠 AI-Based Navigation

---

# 📸 Project Images

```
Images/

Robot Front View

Robot Side View

Complete Wiring

Bluetooth App

Arduino Uno

Motor Driver

Finished Prototype
```

*(Add actual project images in the Images folder.)*

---

# 🎥 Demonstration

A demonstration video should include:

- Bluetooth Pairing
- Forward Motion
- Reverse Motion
- Left Turn
- Right Turn
- Stop Function
- Complete Robot Walkthrough

---

# 🧪 Testing

✔ Bluetooth Connectivity

✔ Motor Rotation

✔ Turning Accuracy

✔ Response Time

✔ Battery Performance

✔ Communication Stability

✔ Range Testing

✔ Continuous Operation

---

# 📚 Learning Outcomes

Through this project you will learn:

- Arduino Programming
- Embedded Systems
- Serial Communication
- Bluetooth Communication
- Motor Driver Interface
- PWM Speed Control
- Differential Drive Robot
- Robot Navigation Basics
- Mobile Application Integration
- Wireless Robotics

---

# 🤝 Contributing

Contributions are welcome!

You can contribute by:

- Improving the code
- Optimizing robot movement
- Adding new Bluetooth commands
- Improving documentation
- Designing a better mobile interface
- Fixing bugs
- Enhancing hardware design

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Author

**Koushik M**

**BE Mechatronics Engineering**

Passionate about Robotics, Embedded Systems, IoT, Automation, AI, and Smart Embedded Solutions.

GitHub:
https://github.com/koushikmvkk-gif

LinkedIn:
https://www.linkedin.com/in/koushik-nair-4556b0291

---

# 🌟 Support

If you found this project useful:

⭐ Star this repository

🍴 Fork the repository

🐛 Report issues

💡 Suggest new features

🤝 Contribute to future improvements

---

<div align="center">

## ⭐ If you like this project, don't forget to Star the Repository!

**Happy Building! 🚗📡🤖**

</div>
