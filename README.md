# PIC16F648A-Avionics-Interface-PCB-24V
Open-source avionics-grade PCB built around the PIC16F648A microcontroller. Features 24V industrial/aviation power input via a DB9 connector, LMC6032 op-amps for analog signal conditioning, LM317/LM7805 voltage regulation, and 5 status LEDs. Designed for robust embedded control and monitoring applications.
# PIC16F648A Avionics Interface PCB

![EasyEDA](https://img.shields.io/badge/Designed_in-EasyEDA-blue)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains the complete hardware design files for a rugged, industrial/avionics interface board based on the **PIC16F648A** microcontroller. Designed by **RED AVIONICS LLC**, this board is built to handle 24V power rails while providing analog signal conditioning and digital control.

![Image](images/pcb_3d_render.png) <!-- Make sure to add your 3D render and PCB shots in an images/ folder -->

## ✨ Project Overview
------------------------------------
<img width="1169" height="1202" alt="Schematic_PIC16F648A_Based_PCB_Designing_2026-05-02" src="https://github.com/user-attachments/assets/7b106c9f-e301-44d2-b36f-2f490f0c85dd" />

--------------------------------------
<img width="585" height="607" alt="PIC16F648A_Based_PCB_Designing_3D_Top_View" src="https://github.com/user-attachments/assets/392f8a19-3882-4fa3-95db-05f792ecc620" />

--------------------------------------
<img width="662" height="602" alt="PIC16F648A_Based_PCB_Designing_3D_Bottom_View" src="https://github.com/user-attachments/assets/1b82a492-70b1-48ad-bb45-88d3af3a7ec0" />

-------------------------------------
<img width="587" height="630" alt="PIC16F648A_Based_PCB_Designing_2D_View" src="https://github.com/user-attachments/assets/99cea47f-620b-4d1d-ba6a-8d80b15b3728" />

--------------------------------------
This board is designed for critical analog and digital interface applications in high-reliability environments. It takes in power and signals via a D-Sub (DB9) connector, regulates the high voltage down to 5V logic, and uses dual op-amps to condition external analog inputs before feeding them into the PIC16F648A MCU.

## 🔧 Key Specifications

*   **Controller:** **PIC16F648A-I/SO** (SOIC-18 package).
*   **Clock Speed:** 16MHz (External crystal).
*   **Power Input:** 24V DC via DB9 connector (DMR-9P).
*   **Voltage Regulation:**
    *   **LM317 (U3):** Provides an adjustable intermediate voltage rail (prob. 10V or 12V, set by R20/R21).
    *   **LM7805 (U4):** Provides stable 5V logic power.
*   **Protection:** 1N4007 (D1, D3) for reverse polarity and flyback protection.
*   **Analog I/O:** 2x **LMC6032IMX/NOPB** (Dual Op-Amp) ICs for signal buffering, filtering, and conditioning.
*   **User Interface:** 5x Red LEDs (LED1-LED5) and a tactile reset switch (SW1).
*   **External Interface:** DB9 connector for robust cable connection + 4-pin header (H1).

## 📂 Repository Structure
```text
/
├── images/                                   # Renders (3D, PCB B&W)
├── Schematic_PIC16F648A_Based_PCB_Designing_2026-05-02.pdf     
├── PCB_PCB_PIC16F648A_Based_PCB_Designing_2026-05-02.pdf             
├── BOM_PIC16F648A_Based_PCB_Designing_2026-05-02.csv       
└── PickAndPlace_PCB_PIC16F648A_Based_PCB_Designing_2026-05-02.csv
