---
layout: project
type: project
image: img/hive11.png
title: "Hive-1 & Hive-2 – Autonomous Swarm Robots"
date: 2024-01 – Present
published: true
labels:
  - Swarm Robotics
  - PCB Design
  - Embedded Systems
  - ESP32
  - Sensor Fusion
summary: "Contributed to custom PCB-based autonomous swarm robots (Hive-1 and Hive-2) featuring onboard sensing, wireless control, AprilTag localization, and coordinated omniwheel mobility."
---



# **Project Overview**

Hive-1 and Hive-2 are custom-designed **autonomous swarm robots** built around a modular PCB architecture using **Arduino Nano ESP32**, omniwheel mobility, and lightweight sensing pipelines.
Both platforms were engineered for synchronized multi-robot experiments, distributed control, and indoor localization.

<div class="text-center p-4">
  <img width="400px" src="../img/hive11.png" class="img-thumbnail">
</div>

---

# **Hive-1: Sensor-Rich Swarm Platform**

**Key Features**

* Contributed to the design of three custom PCBs integrating:

  * Arduino Nano ESP32
  * LiDAR
  * SLAM module
  * 9-axis IMU
* Implemented AprilTag + wheel-odometry localization for coordinated swarm motion
* Developed firmware for synchronized behaviors, wireless communication, and sensor calibration
* Designed the charging dock and power management system

<div class="text-center p-4">
  <img width="400px" src="../img/hive22.png" class="img-thumbnail">
</div>

---

# **Hive-2: Lightweight Micro-Swarm Variant**

Hive-2 retained the same motion and communication system as Hive-1 but removed the LiDAR + SLAM modules to create a lighter, lower-cost platform for large-scale swarm deployments.

**Key Differences**

* Same ESP32-based PCB, IMU, and omniwheel system
* No LiDAR / SLAM → reduced power draw & simplified sensing
* Designed for larger swarms and rapid manufacturing
* Firmware reuse for formation control and coordinated multi-robot behaviors

---

# **Capabilities**

* Coordinated omniwheel motion
* Indoor localization using AprilTags
* Wireless inter-robot communication
* Scalable swarm behaviors (leader–follower, formations, synchronized motion)

---

# **Future Work**

* Add UWB localization
* Shared map construction across the swarm
* Improved inter-robot communication layers
* Publish PCB + firmware open source