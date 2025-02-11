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
4. [Images](#images)
5. [Contributors](#contributors)

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

![OTA Schematic](images/ota_schematic.png)
*Figure 10: Schematic of OTA*

![OTA Testbench](images/ota_testbench.png)
*Figure 11: Schematic of OTA Testbench*

### Main Circuit with Ideal OTA
The main circuit was first simulated with an ideal OTA to verify the design. The gain and bandwidth were measured, and the results are shown below:

![Amplifier Gain with Ideal OTA](images/amplifier_gain_ideal_ota.png)
*Figure 17: Amplifier Gain in dB with Ideal OTA*

### Main Circuit with Real OTA
The main circuit was then simulated with the actual OTA. The results showed a slight deviation from the ideal case due to the limited bandwidth of the OTA.

![Amplifier Gain with Real OTA](images/amplifier_gain_real_ota.png)
*Figure 21: Amplifier Gain in dB with Real OTA*

### Bonus: Different Gains and CMRR
As part of the bonus section, different gains (common mode, differential mode, etc.) and the Common Mode Rejection Ratio (CMRR) were calculated and simulated.

![CMRR Schematic](images/cmrr_schematic.png)
*Figure 34: CMRR Schematic*

---

## Waveform Generator

### Circuit Design
The waveform generator consists of three main stages:
1. **Astable Multivibrator**: Generates a square wave.
2. **Integrator**: Converts the square wave into a triangular wave.
3. **Low-Pass Filter**: Converts the triangular wave into a sine wave.

The circuit was designed to operate at frequencies from 100kHz to 10MHz.

### Simulation Results
The output waveforms for square, triangular, and sine waves at 100kHz and 10MHz are shown below:

![Square Wave at 100kHz](images/square_wave_100kHz.png)
*Figure 50: Square Wave at 100kHz*

![Triangular Wave at 100kHz](images/triangular_wave_100kHz.png)
*Figure 51: Triangular Wave at 100kHz*

![Sine Wave at 100kHz](images/sine_wave_100kHz.png)
*Figure 52: Sine Wave at 100kHz*

---

## Images

Below are the key images from the project:

1. **OTA Schematic**: ![OTA Schematic](images/ota_schematic.png)
2. **OTA Testbench**: ![OTA Testbench](images/ota_testbench.png)
3. **Amplifier Gain with Ideal OTA**: ![Amplifier Gain with Ideal OTA](images/amplifier_gain_ideal_ota.png)
4. **Amplifier Gain with Real OTA**: ![Amplifier Gain with Real OTA](images/amplifier_gain_real_ota.png)
5. **CMRR Schematic**: ![CMRR Schematic](images/cmrr_schematic.png)
6. **Square Wave at 100kHz**: ![Square Wave at 100kHz](images/square_wave_100kHz.png)
7. **Triangular Wave at 100kHz**: ![Triangular Wave at 100kHz](images/triangular_wave_100kHz.png)
8. **Sine Wave at 100kHz**: ![Sine Wave at 100kHz](images/sine_wave_100kHz.png)

---

## Contributors

This project was completed by the following team members:

| ID       | Section | Name                          |
|----------|---------|-------------------------------|
| 9220007  | 1       | ابراهيم ايمن ناهد محمد         |
| 9220022  | 1       | احمد امير يسري ابراهيم         |
| 9220028  | 1       | احمد حسن محمد حسن             |
| 9220247  | 2       | حازم احمد عبدالفتاح حسن       |
| 9220276  | 2       | خالد احمد حامد عبدالعزيز       |
| 9220461  | 2       | عبدالرحمن حاتم نصر يوسف       |

---

For more details, please refer to the project report and simulation files in the repository.
