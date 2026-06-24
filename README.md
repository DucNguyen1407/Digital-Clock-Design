# Digital Clock Design using 74-Series Logic ICs

A 6-digit digital clock project developed as part of the Digital Systems Design course at Hanoi University of Science and Technology. This project implements a complete timekeeping system using discrete logic components without any microprocessors.

## Project Overview
The objective of this project is to design and build a digital clock that displays Hours, Minutes, and Seconds on six 7-segment LED displays. The system is built entirely using combinational and sequential logic circuits, providing hands-on experience with IC-based timing and counting.

## Technical Specifications
* **Core Logic**: 74LS90 (BCD Counter) and 74LS47 (BCD to 7-Segment Decoder).
* **Display**: 6x Common Anode 7-segment LEDs.
* **Time Format**: 24-hour display (HH:MM:SS).
* **Control**: 3 manual push buttons for incrementing Hours, Minutes, and Seconds.
* **Power Supply**: 5V DC.

## System Architecture

The system is organized into five functional blocks:

1. **Clock Generation Block**: Generates a precise 1Hz square wave (1 pulse per second).
2. **Counter Block**: Utilizes **74LS90** ICs to count Seconds (00-59), Minutes (00-59), and Hours (00-23).
3. **Decoder Block**: Uses **74LS47** ICs to convert BCD signals for 7-segment displays.
4. **Display Block**: Consists of six Common Anode 7-segment LEDs with current-limiting resistors.
5. **Power Block**: Stable 5VDC supply.

## Simulation & Design
The circuit logic was fully validated using Proteus software before hardware implementation.

<img width="624" height="404" alt="Picture1" src="https://github.com/user-attachments/assets/9b2c2805-db38-41c4-8318-747dcd99ae38" />

*Figure 1: Proteus Schematic Diagram*

## Hardware Implementation
The physical prototype was assembled on breadboards. The wiring ensures stable signal transmission between the counter stages and the display decoders.

<img width="562" height="749" alt="Picture2" src="https://github.com/user-attachments/assets/233c09b8-84a1-460d-8079-94458b419a78" />

*Figure 2: Final Hardware Prototype*

## Key Learning Outcomes
* Mastering the operation of 74LS90 counter and 74LS47 decoder.
* Understanding logic reset conditions for Modulo-60 and Modulo-24 counters.
* Practical skills in circuit troubleshooting and hardware debugging.

## Contributors
* **Instructor**: Associate Professor, PhD Cuong Quoc Nguyen
* **Student Team**: 
    * Dung Manh Nguyen
    * Duc Minh Nguyen
* **Class**: Control Engineering & Automation (Talent Program)
* **Institution**: School of Electrical and Electronic Engineering (SEEE) - HUST

## Contribution
Contributions are welcome! Please feel free to submit issues or pull requests.
