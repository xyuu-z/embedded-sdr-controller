# Embedded SDR Controller

> Embedded control subsystem for a software-defined radio (SDR) transceiver, featuring a custom PCB, ATmega324PB firmware, and real-time frequency control.

> **University of Toronto | ECE295 Engineering Design Project**

> **Note:** Source code is not included due to University of Toronto academic integrity policies.

---

## Overview

This project was completed as part of the University of Toronto ECE295 Engineering Design course.

Our team designed and built the control subsystem for a software-defined radio (SDR) transceiver. The controller allows users to adjust the output frequency in real time using a rotary encoder while displaying system information on an LCD. It communicates with a Si5351 frequency synthesizer over I²C and provides control signals to downstream RF subsystems.

The project involved the complete embedded hardware development workflow, including schematic design, PCB layout, firmware development, PCB assembly, and hardware validation.

---

## Project Objectives

- Design a custom PCB for the SDR control subsystem
- Develop embedded firmware for the ATmega324PB microcontroller
- Configure the Si5351 frequency synthesizer via I²C
- Display system status on a 1602 LCD
- Enable real-time frequency adjustment from **8 MHz to 16 MHz**
- Produce a manufacturable hardware design

---

## System Architecture

![BlockDiagram](image/blockDiagram.png)

---

## My Contributions

### PCB Design

- Designed the complete schematic and two-layer PCB using **Altium Designer**
- Performed ERC and DRC verification
- Generated manufacturing-ready Gerber files
- Assembled and soldered the PCB

### Embedded Firmware

- Developed polling-based firmware in Embedded C
- Configured the Si5351 frequency synthesizer over I²C
- Controlled the 1602 LCD display
- Implemented rotary encoder input for real-time frequency adjustment

### Team Leadership

- Led a two-person subsystem team
- Coordinated hardware and firmware integration within the transceiver project

---

## Hardware

### PCB

> *(Insert PCB layout screenshot)*

### Schematic

> *(Insert schematic screenshot)*

### Assembled Board

> *(Insert photo of assembled PCB)*

---

## Firmware

The firmware initializes all peripherals before entering a polling loop that continuously:

1. Reads the rotary encoder
2. Calculates the target frequency
3. Updates the Si5351 through I²C
4. Refreshes the LCD display

> *(Insert firmware flowchart here)*

---

## Technical Challenges

### Hardware Integration

The project required integrating multiple peripherals—including the Si5351 frequency synthesizer, LCD, and rotary encoder—into a single embedded controller while maintaining reliable communication over I²C.

### PCB Design

Creating a manufacturable PCB required schematic verification, layout validation, and fabrication-ready design rule checks before assembly.

### Embedded Control

The firmware was designed to provide responsive user interaction while maintaining stable communication with all peripherals.

---

## Demonstration

> *(Insert GIF or short video demonstrating frequency adjustment and LCD updates.)*

---

## Skills Demonstrated

- Embedded Systems
- Embedded C
- PCB Design
- Altium Designer
- Hardware Assembly
- I²C Communication
- Microcontroller Programming
- Hardware Validation

---

## Lessons Learned

This project strengthened my understanding of the complete embedded hardware development process—from schematic capture and PCB layout to firmware implementation and hardware bring-up.

It also reinforced the importance of designing hardware and firmware together as an integrated embedded system.

---

## Repository Contents

```
README.md
images/
docs/
```

---

## Code Availability

The source code for this project is **not publicly available** due to University of Toronto academic integrity policies.

This repository serves as an engineering portfolio documenting the project architecture, hardware design, and development process.
