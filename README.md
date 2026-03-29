# 🚗 Electric Vehicle Modelling with DC Motor — Simulink Model & Report

> Complete EV simulation: Lithium-Ion Battery → H-Bridge Controller → DC Motor → Vehicle Dynamics → Drive Cycle Tracking with Regenerative Braking

![Status](https://img.shields.io/badge/Status-Completed-3fb950?style=flat-square)
![Tool](https://img.shields.io/badge/Tool-MATLAB%20%7C%20Simulink-blue?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Electric%20Vehicles%20%7C%20EV%20Powertrain-f0a500?style=flat-square)
![Motor](https://img.shields.io/badge/Motor-DC%20Permanent%20Magnet-purple?style=flat-square)
![Controller](https://img.shields.io/badge/Controller-H--Bridge%20%7C%20PWM-red?style=flat-square)
![Braking](https://img.shields.io/badge/Feature-Regenerative%20Braking-green?style=flat-square)

---

## 📌 Overview

This repository contains a **complete Electric Vehicle (EV) simulation** built in **MATLAB Simulink**, along with a **detailed project report (PDF)** covering system design, component modelling, and simulation results.

The model simulates a DC motor-driven EV following a standard drive cycle — covering battery discharge, motor control via H-Bridge, vehicle dynamics (mass, drag, friction), tire modelling, and regenerative braking.

**Drive Cycle Input → Longitudinal Driver → H-Bridge Controller → DC Motor → Gearbox → Differential → Tires → Vehicle Body → Speed/SOC Output**


---

## 🚀 System Architecture

| # | Component | Function |
|---|-----------|----------|
| 1 | Lithium-Ion Battery | Supplies electrical energy to the motor |
| 2 | H-Bridge Motor Controller | Controls motor speed via PWM (Averaged mode) |
| 3 | DC Motor (Permanent Magnet) | Converts electrical energy into mechanical torque |
| 4 | Gearbox & Differential | Transfers torque to the driving wheels |
| 5 | Tires (Magic Formula) | Models tire-road interaction with slip dynamics |
| 6 | Vehicle Body | Accounts for mass, aerodynamic drag, road incline |
| 7 | Longitudinal Driver | Tracks reference speed — generates accel/brake commands |
| 8 | Regenerative Braking | Feeds energy back to battery during deceleration |

---

## 📈 Results Summary

| Output | Result |
|--------|--------|
| Reference vs Actual Speed | Vehicle closely tracks the drive cycle input |
| Total Distance Covered | **18.71 km** over the full simulation run |
| Battery SOC at End | **~81.39%** (started at 100%) |
| Regenerative Braking | SOC increases slightly during heavy deceleration phases |
| Simulation Time | 2474 seconds (full drive cycle duration) |

---

## 📄 About the Report

The included **PDF report** covers:

| Section | Content |
|---------|---------|
| Abstract | Project summary and objectives |
| Introduction | Why EV modelling matters, role of DC motors |
| System Overview | Block diagram and signal flow |
| Components | Battery, controller, vehicle body, DC motor, tires, driver — each explained |
| Simulation | Model setup, solver config, scope connections |
| Results & Graphs | Speed tracking, distance, SOC, current & voltage plots |
| Conclusion | Key findings, regenerative braking observations |

---

## 🔥 Key Features

- ✅ Full EV powertrain modelled — battery to wheels
- ✅ DC Permanent Magnet motor with H-Bridge PWM control
- ✅ Realistic vehicle dynamics — mass, drag, road incline
- ✅ Magic Formula tire model for tire-road interaction
- ✅ Longitudinal driver for drive cycle speed tracking
- ✅ Regenerative braking enabled — energy recovery during deceleration
- ✅ Battery SOC monitoring throughout the run
- ✅ Detailed project report (PDF) with graphs and analysis

---

## 🗂️ Repository Contents

EV-DC-Motor-Simulink

* Final_electric_vehicle_project.slx - Complete Simulink model
* Report Electric vehicle modelling.pdf - Detailed project report
* README.md


**Requirements:** MATLAB R2022a or later · Simulink · Simscape Electrical · Simscape Driveline

---

## 🔗 How to Run

1. Clone or download this repository
2. Open `Final_electric_vehicle_project.slx` in MATLAB Simulink
3. Click **Run** (Stop Time: 2474s — full drive cycle)
4. Check scopes for speed tracking, SOC, current, voltage, and distance
5. Read `Report Electric vehicle modelling.pdf` for full analysis

---
