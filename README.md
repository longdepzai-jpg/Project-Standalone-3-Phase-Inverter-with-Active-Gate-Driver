# Standalone 3-Phase Inverter with Active Gate Driver (AGD)

## Overview

Silicon Carbide (SiC) MOSFETs offer superior efficiency and switching speeds for power converters. However, driving these advanced wide-bandgap semiconductors at high frequencies introduces critical hardware challenges:
* Severe voltage overshoots ($\text{dv/dt}$)
* Crosstalk phenomena in bridge configurations
* High-frequency switching losses
* Electromagnetic interference (EMI)

This project focuses on the hardware design of a standalone 3-phase inverter utilizing Active Gate Driver (AGD) technology to safely and efficiently harness the performance of SiC MOSFETs.

## Objectives

The main goals of this project are:
* Study the switching characteristics and parasitic behaviors of SiC MOSFETs
* Design an Active Gate Driver circuit to dynamically control the gate charging/discharging process
* Mitigate voltage overshoots, crosstalk, and switching losses during high-frequency operation
* Validate hardware reliability under real-world operating conditions

*This project focuses strictly on power electronics hardware design, high-frequency circuit tuning, and physical validation.*

## Methodology

The hardware design process follows these steps:
1. Analyze SiC MOSFET datasheet parameters and calculate driving requirements
2. Design the Active Gate Driver topology and select high-speed isolation components
3. Optimize the PCB layout to minimize parasitic inductances in the gate loop and power loop
4. Fabricate the standalone inverter prototype
5. Tune the AGD circuit parameters (resistors, active pull-down logic)
6. Perform rigorous experimental validation

The hardware is validated using:
* **Oscilloscopes:** Capturing and analyzing PWM signals, gate-source voltages ($V_{gs}$), and phase outputs
* **Precise Circuit Tuning:** Iterative adjustments to minimize switching losses
