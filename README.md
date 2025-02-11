# IC Project: Amplifier Design & Waveform Generator

This repository contains the design and simulation of an amplifier and waveform generator as part of an IC design project. The project is divided into two main parts: **Amplifier Design** and **Waveform Generator**.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Amplifier Design](#amplifier-design)
   - [Initial Design](#initial-design)
   - [Tuning](#tuning)
   - [OTA Design](#ota-design)
   - [Main Circuit with Ideal OTA](#main-circuit-with-ideal-ota)
   - [Main Circuit with Real OTA](#main-circuit-with-real-ota)
   - [Bonus: Different Gains and CMRR](#bonus-different-gains-and-cmrr)
3. [Waveform Generator](#waveform-generator)
   - [Circuit Design](#circuit-design)
   - [Simulation Results](#simulation-results)
4. [Contributors](#contributors)

---

## Project Overview

This project focuses on the design and simulation of an Operational Transconductance Amplifier (OTA) and a waveform generator. The OTA is designed to meet specific gain and bandwidth requirements, while the waveform generator is capable of producing square, triangular, and sine waves at frequencies ranging from 100kHz to 10MHz.

---

## Amplifier Design

### Initial Design
The initial design of the main circuit was based on the following specifications:
- **Gain**: 90 dB
- **Bandwidth**: 1 MHz
- **GBW**: 32.623 GHz

The design process involved calculating the required transconductance (gm), current (ID), and sizing of the MOSFETs.

### Tuning
After the initial design, tuning was performed to meet the required specifications. This involved adjusting the width and length of the MOSFETs to achieve the desired gain and bandwidth.

### OTA Design
The OTA was designed with the following specifications:
- **Gain**: 70 dB
- **Bandwidth**: 20 MHz
- **GBW**: 1.4 GHz

The OTA schematic and testbench are shown below:

![image](https://github.com/user-attachments/assets/da8dca94-0880-430e-9132-931d584b060d)

*Figure 10: Schematic of OTA*

![image](https://github.com/user-attachments/assets/9b2b06b3-fdd6-416c-8298-7ba93a952351)

*Figure 11: Schematic of OTA Testbench*

### Main Circuit with Ideal OTA
The main circuit was first simulated with an ideal OTA to verify the design. The gain and bandwidth were measured, and the results are shown below:

![image](https://github.com/user-attachments/assets/d427af0c-7e4d-4628-9199-e6a127659abc)

*Figure 17: Amplifier Gain in dB with Ideal OTA*

### Main Circuit with Real OTA
The main circuit was then simulated with the actual OTA. The results showed a slight deviation from the ideal case due to the limited bandwidth of the OTA.

![image](https://github.com/user-attachments/assets/517c290c-c070-4000-92fe-a17a5b2844f5)

*Figure 21: Amplifier Gain in dB with Real OTA*

### Bonus: Different Gains and CMRR
As part of the bonus section, different gains (common mode, differential mode, etc.) and the Common Mode Rejection Ratio (CMRR) were calculated and simulated.

![image](https://github.com/user-attachments/assets/2b112ad9-0cf2-466b-8c50-b9f22001fd78)

*Figure 34: CMRR Schematic*

---

## Waveform Generator

### Circuit Design
The waveform generator consists of three main stages:
1. **Astable Multivibrator**: Generates a square wave.
2. **Integrator**: Converts the square wave into a triangular wave.
3. **Low-Pass Filter**: Converts the triangular wave into a sine wave.
![image](https://github.com/user-attachments/assets/2b26974c-3250-482d-9592-2e394a287464)

*Figure 46: The Schematic for the circuit*

The circuit was designed to operate at frequencies from 100kHz to 10MHz.

### Simulation Results
The output waveforms for square, triangular, and sine waves at 100kHz and 10MHz are shown below:

![image](https://github.com/user-attachments/assets/73d41ec9-f055-4f19-ba67-6aecdc0d7661)

*Figure 50: Square Wave at 100kHz*

![image](https://github.com/user-attachments/assets/f81c1e55-633b-4055-b285-1fce824c5b96)

*Figure 51: Triangular Wave at 100kHz*

![image](https://github.com/user-attachments/assets/07cb65b0-2f53-4963-a252-a42787db959a)

*Figure 52: Sine Wave at 100kHz*

---

## Contributors

This project was completed by the following team members:

| ID       | Section | Name                          |
|----------|---------|-------------------------------|
| 9220007  | 1       | Ibrahim Ayman Nahed         |
| 9220022  | 1       | Ahmed Amir Youssry         |
| 9220028  | 1       | Ahmed Hassan Mohamed             |
| 9220247  | 2       | Hazem Ahmed Abdelfattah       |
| 9220276  | 2       | Khaled Ahmed Hamed       |
| 9220461  | 2       | Abdelrahman Hatem Nasr       |


