# 🤖 Line Following Robot Using Arduino Uno

## 📌 Project Overview

The **Line Following Robot** is an autonomous robotic vehicle designed to follow a predefined path, usually a black line on a white surface, using IR (Infrared) sensors.

The robot uses an Arduino Uno as its main controller. The IR sensors detect the line, and the Arduino processes the sensor signals to control the motors through a motor driver module.

This project demonstrates the practical implementation of embedded systems, robotics, sensor interfacing, and motor control.

## 🎯 Objectives

- To design an autonomous line-following robot.
- To understand IR sensor interfacing with Arduino Uno.
- To implement motor control using a motor driver.
- To understand basic robotics and embedded system concepts.
- To develop a robot that can follow a predefined path without manual control.

## 🛠️ Components Required

| Component | Quantity |
|---|---:|
| Arduino Uno | 1 |
| IR Sensors | 2 |
| Motor Driver Module (L298N) | 1 |
| DC Gear Motors (TT Motors) | 4 |
| Robot Chassis | 1 |
| Wheels | 4 |
| Battery | 1 |
| Jumper Wires | As required |

## 🔌 Circuit Connections

### IR Sensor Connections

| IR Sensor | Arduino Uno |
|---|---|
| Left IR Sensor OUT | Digital Pin 2 |
| Right IR Sensor OUT | Digital Pin 3 |
| VCC | 5V |
| GND | GND |

### Motor Driver Connections

| Motor Driver Pin | Arduino Uno |
|---|---|
| ENA | Pin 11 |
| IN1 | Pin 10 |
| IN2 | Pin 9 |
| ENB | Pin 6 |
| IN3 | Pin 8 |
| IN4 | Pin 7 |

**Note:** The motor driver controls the direction and speed of the DC motors. The left and right motors are connected to the respective motor driver output terminals.

## ⚙️ Working Principle

The robot uses two IR sensors to detect the black line on the surface.

1. **Line Detection:** IR sensors detect the difference between black and white surfaces.
2. **Signal Processing:** The sensors send digital signals to the Arduino Uno.
3. **Decision Making:** Arduino processes the sensor inputs and determines the robot's movement.
4. **Motor Control:** The motor driver receives signals from Arduino and controls the motors.
5. **Movement:** The robot moves forward, turns left, or turns right depending on the detected line.

## 🚦 Movement Logic

| Left Sensor | Right Sensor | Robot Movement |
|---|---|---|
| White | White | Move Forward |
| Black | White | Turn Left |
| White | Black | Turn Right |
| Black | Black | Stop / Intersection handling |

*Note: Sensor output logic may vary depending on the IR sensor module. Adjust the logic according to your sensor calibration.*

## 💻 Technologies Used

- **Programming Language:** Embedded C / Arduino C++
- **Microcontroller:** Arduino Uno
- **IDE:** Arduino IDE
- **Sensors:** Infrared (IR) Sensors
- **Motor Control:** L298N Motor Driver

## 🔄 Project Workflow

1. Power on the Arduino Uno.
2. IR sensors continuously scan the surface.
3. Sensor signals are transmitted to the Arduino.
4. Arduino determines the robot's direction.
5. Motor driver controls the motors accordingly.
6. The robot follows the predefined black line.

## 📚 Applications

- Autonomous mobile robots
- Industrial automation
- Automated material transportation
- Robotics learning and experimentation
- Embedded systems applications

## 🚀 Future Improvements

- Implement PID control for smoother movement.
- Add additional IR sensors for improved line detection.
- Implement obstacle detection using ultrasonic sensors.
- Improve navigation at sharp turns and intersections.
- Add wireless monitoring and control.

## 🎓 Learning Outcomes

Through this project, we gained practical knowledge of:

- Arduino programming and interfacing.
- IR sensor operation.
- DC motor control.
- Motor driver interfacing.
- Basic autonomous navigation.
- Hardware integration and troubleshooting.

## 👩‍💻 Project Information

**Project Name:** Line Following Robot Using Arduino Uno

**Domain:** Robotics and Embedded Systems

**Platform:** Arduino Uno

**Project Type:** Hardware-Based Mini Project

---

⭐ If you find this project interesting, consider giving this repository a star!

**Built with Arduino, sensors, and robotics! 🤖**
