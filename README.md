# Digital Clock Design using 74-Series Logic ICs

[cite_start]A 6-digit digital clock project developed as part of the Digital Systems Design course at Hanoi University of Science and Technology[cite: 1, 3, 5]. [cite_start]This project implements a complete timekeeping system using discrete logic components without any microprocessors[cite: 5].

## 📌 Project Overview
[cite_start]The objective of this project is to design and build a digital clock that displays Hours, Minutes, and Seconds on six 7-segment LED displays[cite: 31, 33]. [cite_start]The system is built entirely using combinational and sequential logic circuits, providing hands-on experience with IC-based timing and counting[cite: 5, 40].

## 🛠 Technical Specifications
* [cite_start]**Core Logic**: 74LS90 (BCD Counter) and 74LS47 (BCD to 7-Segment Decoder)[cite: 48, 70].
* [cite_start]**Display**: 6x Common Anode 7-segment LEDs[cite: 31, 116].
* [cite_start]**Time Format**: 24-hour display (HH:MM:SS)[cite: 33, 66].
* [cite_start]**Control**: 3 manual push buttons for incrementing Hours, Minutes, and Seconds[cite: 36].
* [cite_start]**Power Supply**: 5V DC[cite: 35, 121].

## 🏗 System Architecture

[cite_start]The system is organized into five functional blocks[cite: 39]:

### 1. Clock Generation Block
[cite_start]Generates a precise 1Hz square wave (1 pulse per second)[cite: 42, 43]. [cite_start]This serves as the master clock for the entire system to ensure accurate timekeeping[cite: 45].

### 2. Counter Block
[cite_start]Utilizes **74LS90** ICs to perform frequency division and counting[cite: 48, 49]:
* [cite_start]**Seconds/Minutes**: Counts from 00 to 59, resetting at the 60th pulse to carry over to the next unit[cite: 66].
* [cite_start]**Hours**: Counts from 00 to 23, with a logic reset at "24" to return to 00[cite: 66].

### 3. Decoder Block
[cite_start]Uses **74LS47** ICs to convert the 4-bit BCD output from the counters into signals compatible with 7-segment displays[cite: 71, 106].

### 4. Display Block
[cite_start]Consists of six 7-segment LEDs (Common Anode)[cite: 108, 112]. [cite_start]Current-limiting resistors (220Ω) are placed between the decoder and each LED segment for protection[cite: 107].

### 5. Power Block
[cite_start]A 5V-2A Adapter converts 220VAC power into a stable 5VDC supply for the TTL logic components[cite: 121].

## 🚀 Implementation
The project followed a two-stage development process:
1.  [cite_start]**Simulation**: Validated the schematic logic using **Proteus** software[cite: 24, 123].
2.  [cite_start]**Hardware Assembly**: Constructed the physical circuit on breadboards for final testing[cite: 25, 125].

## 👥 Contributors
* [cite_start]**Instructor**: PGS.TS Nguyễn Quốc Cường [cite: 6]
* **Student Team**: 
    * [cite_start]Nguyễn Mạnh Dũng (20232026) [cite: 7]
    * [cite_start]Nguyễn Minh Đức (20230005) [cite: 7]
* [cite_start]**Class**: CTTN – Control Engineering & Automation, K68 [cite: 8]
* [cite_start]**Institution**: School of Electrical and Electronic Engineering (SEEE) - HUST [cite: 1, 2]
