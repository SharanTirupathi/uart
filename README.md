# UART Controller with Configurable FIFO and Error Detection using Verilog HDL

## Table of Contents

- Overview
- Features
- System Architecture
- Project Structure
- Module Description
- RTL Schematic
- Simulation Results
- Timing Analysis
- Power Analysis
- Tools Used
- Applications
- Future Improvements
- Contributors
- License

## 📖 Overview

This project implements a configurable UART (Universal Asynchronous Receiver Transmitter) Controller in Verilog HDL with an integrated parameterized FIFO buffer and comprehensive error detection mechanisms. The design supports asynchronous serial communication while providing configurable UART parameters such as baud rate, data bits, parity mode, stop bits, and FIFO depth.

The project was developed using Xilinx Vivado and verified through simulation, RTL analysis, timing analysis, and power analysis.

---

## ✨ Features

- UART Transmitter
- UART Receiver
- Parameterized FIFO Buffer (Configurable Depth)
- Configurable Baud Rate
- Configurable Data Width
- Configurable Stop Bits
- Configurable Parity (Even/Odd/None)
- Baud Rate Generator
- FIFO Overflow Detection
- Parity Error Detection
- Frame Error Detection
- RTL Simulation using Xilinx Vivado
- Synthesizable Verilog HDL Design

---

## 🏗️ System Architecture

<p align="center">
<img src="images/architecture.png" width="800">
</p>

---

## 📂 Project Structure

```
UART-Controller-with-Configurable-FIFO-and-Error-Detection
│
├── docs/
│   ├── uart_final.pdf
│   └── ieee_paper.pdf
│
├── images/
│   ├── architecture.png
│   ├── transmitter.png
│   ├── receiver.png
│   ├── fifo.png
│   ├── baudrate_generator.png
│   ├── rtl_schematic.png
│   ├── transmitted_waveform.png
│   ├── receiving_waveform.png
│   ├── timing_analysis.png
│   ├── power_analysis.png
│   ├── testcase_console1.png
│   └── testcase_console2.png
│
├── rtl/
│   ├── baud_gen.v
│   ├── sync_fifo.v
│   ├── uart_rx.v
│   ├── uart_tx.v
│   └── uart_top.v
│
├── tb/
│   └── uart_tb.v
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🧩 Module Description

## UART Transmitter

<p align="center">
<img src="images/transmitter.png" width="700">
</p>

Responsible for serial transmission of parallel data.

Features:

- Configurable Data Length
- Configurable Stop Bits
- Configurable Parity
- FSM Controlled Transmission

---

## UART Receiver

<p align="center">
<img src="images/receiver.png" width="700">
</p>

Responsible for receiving asynchronous serial data.

Features:

- Start Bit Detection
- Bit Sampling Logic
- Shift Register
- Parity Checking
- Frame Error Detection

---

## Baud Rate Generator

<p align="center">
<img src="images/baudrate_generator.png" width="500">
</p>

Generates baud enable ticks from the system clock.

---

## Configurable FIFO

<p align="center">
<img src="images/fifo.png" width="650">
</p>

The FIFO is parameterized and supports configurable depth.

Features:

- Configurable FIFO Depth
- Write Pointer
- Read Pointer
- Full Flag
- Empty Flag
- Overflow Detection

---

## 🖥️ RTL Schematic

<p align="center">
<img src="images/rtl_schematic.png" width="850">
</p>

---

### 📊 Simulation Results

## UART Transmission

<p align="center">
<img src="images/transmitted_waveform.png" width="850">
</p>

---

## UART Receiver

<p align="center">
<img src="images/receiving_waveform.png" width="850">
</p>

---

## Test Case 1

<p align="center">
<img src="images/testcase_console1.png" width="850">
</p>

---

## Test Case 2

<p align="center">
<img src="images/testcase_console2.png" width="850">
</p>

---

## ⏱️ Timing Analysis


<p align="center">
<img src="images/timing_analysis.png" width="850">
</p>

---

## ⚡ Power Analysis

<p align="center">
<img src="images/power_analysis.png" width="850">
</p>

---

## 🛠️ Tools Used

- Verilog HDL
- Xilinx Vivado
- Xilinx Simulator (XSim)
- FPGA Design Flow
- RTL Design

---

## 🚀 Applications

- Embedded Systems
- FPGA-Based Communication Systems
- Industrial Communication
- Serial Data Transfer
- ASIC/FPGA Prototyping
- UART-Based Peripheral Interfaces

---

## 🔮 Future Improvements

- AXI Interface Support
- DMA Support
- Interrupt Controller
- UVM Verification Environment
- SystemVerilog Assertions
- Low-Power Optimization
- ASIC Physical Design Implementation

---

## 👥 Contributors

- D. Rishith
- T. Sai Sharan
- K. Shiva Kalyan

---

# Acknowledgement

This project was developed as a Mini Project for the Department of Electronics and Communication Engineering, Chaitanya Bharathi Institute of Technology (CBIT), Hyderabad.

---

## 📜 License

This project is released under the MIT License.
