---
layout: project
type: project
image: img/urc2025.png
title: "Team RoSE – Mars Rover Avionics & Power Systems"
date: 2022-01 – Present
published: true
labels:
  - Robotics
  - Mars Rover
  - PCB Design
  - Power Electronics
  - ROS 2
  - Autonomous Systems
summary: "As Avionics Lead for Team RoSE, I design custom PCB boards, high-current power electronics, and custom battery packs for a fully autonomous Mars Rover competing in the University Rover Challenge."
---



# Team Overview

Team **Robotic Space Exploration (RoSE)** is a student engineering organization designing, building, and testing a fully autonomous Mars Rover for the **University Rover Challenge (URC)**.
In 2024, we advanced to the URC Finals, ranking among the **top 36 teams out of 120+ universities worldwide**.

To learn more, visit the official website: [https://teamrosehawaii.com](https://teamrosehawaii.com)

### **Project Video**

<div class="text-center p-4">
  <iframe 
    src="https://www.youtube.com/embed/bVW3kchtqlg"
    width="560"
    height="315"
    frameborder="0"
    allow="autoplay; encrypted-media; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>

---

# My Role — Avionics Lead

As **Avionics Lead**, I am responsible for the rover’s electrical and embedded systems, including:

* High-current power architecture
* Battery system engineering
* Custom PCB design
* Embedded microcontrollers
* Sensor fusion (IMU + cameras)
* ROS 2 integration
* System reliability and safety

---

# Key Engineering Contributions

## **1. Custom Rover Motherboard (2024–2025 Build)**

A new unified avionics motherboard integrating:

* Dual Arduino Nano ESP32 microcontrollers
* Dual RoboClaw motor controllers
* 9-axis IMU
* Regulated power stages & communication buses
* Thermal and high-current routing optimization

**Purpose:** simplify wiring, improve reliability, and centralize rover electronics.

---

## **2. High-Current Power System**

* Designed the DC power stage for four regulated 12 V / 7 A rails
* Integrated IC-based battery-level and voltage monitoring
* Implemented overcurrent protection with fused outputs
* Engineered modular harnesses for rapid field servicing

**Result:** Stable power delivery during high-load terrain traversal & drive motor stalls.

---

## **3. 8S–4P Li-ion Battery Pack (530 Wh)**

* Custom-designed 8S–4P 21700 Li-ion pack
* Integrated Battery Management System (BMS) for protection & balancing
* Provides ~30V nominal, 530 Wh, and 3+ hours of runtime
* Tested under URC-level current spikes and environmental stress

<div class="text-center p-4">
  <img width="500px" src="../img/BatteryDesign.png" class="img-thumbnail">
</div>

---

## **4. Sensor Fusion & ROS 2 Navigation Integration**

* Integrated IMU and vision modules for improved localization
* Contributed to integrate ROS 2 pipelines for navigation
* Enabled autonomy required for the Autonomous Navigation Mission

**Result:** Robust localization in rough outdoor terrain.

---

# Materials & Methods

### **Electrical Architecture**

* Custom PCBs for battery protection, distribution, and regulation
* High-current wiring, fusing, and connectorization
* Jetson Xavier compute integration
* Modular harnesses for rapid assembly and field repairs

<div class="text-center p-4">
  <img width="300px" src="../img/PDB500.png" class="img-thumbnail">
</div>

---

# Results

* Rover achieved 3+ hour runtimes during field missions
* Successfully completed URC 2024 missions, ranking in the top 36 globally
* Improved wiring reliability through modular connectors & shortened harness paths
* Achieved consistent performance during URC practice missions

---

# Future Work

* Next-generation high-discharge battery pack
* Integration of **Flipsky BMS**
* Breakout PCBs for arm & payload subsystems
* Full avionics integration for URC 2025 competition rover

<div class="text-center p-4">
  <img width="300px" src="../img/FlipskyBMS.png" class="img-thumbnail">
</div>

---

# Conclusion

Guided by results from the 2024 URC Finals, we are building an entirely new electrical and embedded architecture for the 2025 rover—designed for higher reliability, better autonomy performance, improved modularity, and maintainability.
Major subsystems are nearing completion, with full-system testing beginning next semester.

---

# Acknowledgements

* UH College of Engineering
* SOEST, HSFL, HIGP
* UROP Program
* Faculty Advisors
* Protocase
* Team RoSE alumni and supporters

---

