# Digital Clock Design using 74-Series Logic ICs

A 6-digit digital clock project developed as part of the Digital Systems Design course at Hanoi University of Science and Technology. This project implements a complete timekeeping system using discrete logic components without any microprocessors.

## 📌 Project Overview
The objective of this project is to design and build a digital clock that displays Hours, Minutes, and Seconds on six 7-segment LED displays. The system is built entirely using combinational and sequential logic circuits, providing hands-on experience with IC-based timing and counting.

## 🛠 Technical Specifications
* **Core Logic**: 74LS90 (BCD Counter) and 74LS47 (BCD to 7-Segment Decoder).
* **Display**: 6x Common Anode 7-segment LEDs.
* **Time Format**: 24-hour display (HH:MM:SS).
* **Control**: 3 manual push buttons for incrementing Hours, Minutes, and Seconds.
* **Power Supply**: 5V DC.

## 🏗 System Architecture

The system is organized into five functional blocks:

### 1. Clock Generation Block
Generates a precise 1Hz square wave (1 pulse per second). This serves as the master clock for the entire system to ensure accurate timekeeping.

### 2. Counter Block
Utilizes **74LS90** ICs to perform frequency division and counting:
* **Seconds/Minutes**: Counts from 00 to 59, resetting at the 60th pulse to carry over to the next unit.
* **Hours**: Counts from 00 to 23, with a logic reset at "24" to return to 00.

### 3. Decoder Block
Uses **74LS47** ICs to convert the 4-bit BCD output from the counters into signals compatible with 7-segment displays.

### 4. Display Block
Consists of six 7-segment LEDs (Common Anode). Current-limiting resistors (220Ω) are placed between the decoder and each LED segment for protection.

### 5. Power Block
A 5V-2A Adapter converts 220VAC power into a stable 5VDC supply for the TTL logic components.

## 🚀 Implementation
The project followed a two-stage development process:
1.  **Simulation**: Validated the schematic logic using **Proteus** software.
2.  **Hardware Assembly**: Constructed the physical circuit on breadboards for final testing.

## 👥 Contributors
* **Instructor**: PGS.TS Nguyễn Quốc Cường
* **Student Team**: 
    * Nguyễn Mạnh Dũng (20232026)
    * Nguyễn Minh Đức (20230005)
* **Class**: CTTN – Control Engineering & Automation
* **Institution**: School of Electrical and Electronic Engineering (SEEE) - HUST
