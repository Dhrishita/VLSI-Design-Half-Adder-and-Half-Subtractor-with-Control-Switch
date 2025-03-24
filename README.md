# VLSI-Design-Half-Adder-and-Half-Subtractor-with-Control-Switch
This project is a VLSI design and implementation of a Half Adder and Half Subtractor with a Control Switch. The circuit allows switching between addition and subtraction operations using a single control switch. The design involves Boolean equation optimization, gate-level schematic, transistor-level CMOS implementation, stick diagrams, and layout creation using Microwind.


# Embedded-Smart-Irrigation-System

The Smart Irrigation System is designed to automate the process of watering plants based on soil moisture levels. By utilizing sensors and IoT technologies like the ESP8266, this system provides efficient water usage by activating the water pump when necessary. The system also uses Blynk App to monitor environmental conditions such as temperature and humidity, allowing users to receive updates and manage the irrigation system remotely.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Optimized Boolean Equations](#Optimized-Boolean-Equations)
- [Gate-Level Design](#Gate-Level-Design)
- [Transistor-Level Schematic](#Transistor-Level-Schematic)
- [Stick Diagram](#Stick-Diagram)
- [CMOS Implementation](#CMOS-Implementation)
- [Layout Design using Microwind](#Layout-Design-using-Microwind)
- [Performance Analysis](#Performance-Analysis)
- [Contact](#contact)

## Introduction

A Half Adder and Half Subtractor are fundamental arithmetic circuits used in digital systems for adding and subtracting single-bit binary numbers. This project integrates both operations into a single circuit using a control switch.
- **Adder Functionality:** Adds two single-bit numbers
- **Subtractor Functionality:** Subtracts one-bit numbers using the 1’s complement technique
- **Control Switch:**
    - M = 0 → Circuit acts as Half Adder
    - M = 1 → Circuit acts as Half Subtractor

## Features

- Optimized Boolean Logic for Half Adder and Half Subtractor
- Gate-Level Implementation with XOR, AND gates
- Transistor-Level Schematic for CMOS Implementation
- Stick Diagram Representation
- Microwind Layout Design
- Rise Time, Fall Time, and Propagation Delay Analysis
- Low Power Consumption Design

## Optimized Boolean Equations

- For Sum (S) and Difference (D):
  ```bash
   S/D = A ⊕ B
  
- For Carry (C) and Borrow (B):
  ```bash
   C = AB
   B = A'B

- For optimized circuit with control switch:
  ```bash
   C/B = (A ⊕ M)B = (A'M + AM')B

## Gate-Level Design

The circuit is implemented using:
- XOR Gates for sum/difference calculation
- AND Gate for carry generation
- Inverters for logical negations

<img width="422" alt="Fig" src="https://github.com/user-attachments/assets/ff9a44f0-d25f-4f63-b57e-1bbe7b361cc1" />

## Transistor-Level Schematic

CMOS Implementation

- To achieve low power consumption, the circuit is designed using CMOS logic:
  - PMOS Network: Implements logic HIGH states
  - NMOS Network: Implements logic LOW states

- For Sum and Difference
  - Using De Morgan’s Theorem, the optimized CMOS equations are derived:
    ```bash
    P = S/D = A'B + AB'
    F = P' = (A'B + AB')' = (A+B')(A'+B) = A'B' + AB

<img width="264" alt="T" src="https://github.com/user-attachments/assets/7ef0c127-dac7-4a2a-b411-f958b579e093" />

- For Carry and Borrow
  - Using De Morgan’s Theorem, the optimized CMOS equations are derived:
    ```bash
    Y=Q’=((A’M+AM’)B)’
    =(A’M+AM’)’+B’
    =A’M’+AM+B’

<img width="304" alt="yo" src="https://github.com/user-attachments/assets/8c2b3df0-53df-472e-a9af-359b00687269" />

## Stick Diagram

The stick diagram is drawn using standard VLSI color coding for:

- For Sum and Difference

<img width="423" alt="sum" src="https://github.com/user-attachments/assets/c681ca1b-6ced-401b-8233-0ef297ec7173" />

- For Carry and Borrow

<img width="444" alt="Borrow" src="https://github.com/user-attachments/assets/1eceaac1-b08b-4972-b189-de9eca4439ee" />

- Polysilicon (Red)
- Metal (Blue)
- Diffusion (Green)

This helps in visualizing the layout before actual fabrication.


## 
   
## Contact
If you have any questions or suggestions, feel free to open an issue or contact:
Dhrishita Parve: dhrishitap18@gmail.com
