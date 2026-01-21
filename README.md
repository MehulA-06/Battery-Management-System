# Digital Twin–Enabled Battery Management System (Na-Ion)

This project implements a **Digital Twin–based Battery Management System (BMS)** for **Sodium-Ion (Na-ion) batteries**, combining physics-based modeling, state estimation, and machine-learning-based Remaining Useful Life (RUL) prediction.

The system enables accurate monitoring of battery states and predictive diagnostics for next-generation energy storage applications.


## Overview

The Digital Twin framework integrates:
- A **physics-based electro-thermal battery model** developed in COMSOL
- A **MATLAB/Simulink-based BMS**
- **Kalman filter–based state estimation**
- **Machine learning–based RUL prediction**

COMSOL and Simulink are coupled using **LiveLink** to enable real-time co-simulation.


## Key Features

- Sodium-Ion battery modeling using electrochemical principles
- State of Charge (SOC) estimation using Extended Kalman Filter (EKF)
- State of Health (SOH) estimation using internal resistance degradation
- State of Energy (SOE) estimation
- Digital Twin–generated degradation data
- Remaining Useful Life (RUL) prediction using Random Forest regression


## System Architecture

- **Battery Model**  
  - 1D electrochemical DFN (P2D) model
  - Single-cell model scaled to a **6s2p battery pack**

- **BMS Layer (Simulink)**  
  - Equivalent circuit (Thevenin-based) model
  - SOC, SOH, and SOE estimation algorithms
  - Protection and monitoring logic

- **RUL Prediction**
  - Degradation data generated from Digital Twin
  - Random Forest regression for long-term life prediction


## Tools & Technologies

- COMSOL Multiphysics
- MATLAB / Simulink
- Simscape Battery / Battery Builder
- Extended Kalman Filter (EKF)
- Machine Learning (Random Forest)


## Applications

- Battery Management Systems (BMS)
- Electric vehicles
- Grid-scale energy storage
- Predictive maintenance
- Digital Twin–based energy systems


## Future Work

- Particle Filter–based RUL estimation
- Hardware-in-the-Loop (HIL) testing
- Embedded BMS implementation
- Thermal management and cooling integration
