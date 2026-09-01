#  Autonomous Differential Drive Mobile Robot (ROS 2)

A complete mobile robot simulation and hardware implementation built using **ROS 2**, based on the *Articulated Robotics* tutorial series.

---

##  Project Overview
This repository contains the complete codebase, URDF descriptions, simulation worlds, navigation, and hardware control configurations for building a differential drive robot.

###  Key Features / Roadmap
- [x] **URDF & Xacro Modeling:** 3D robot design with modular link & joint structures.
- [x] **Robot State Publisher:** Visualizing robot transformations in RViz.
- [ ] **Gazebo Simulation:** Physics-based world and sensor integration.
- [ ] **Sensor Integration:** LiDAR, Depth Camera, and IMU setup.
- [ ] **ros2_control & Teleoperation:** Real-time motor velocity control.
- [ ] **SLAM (slam_toolbox):** 2D mapping and localization.
- [ ] **Autonomous Navigation (Nav2):** Path planning and obstacle avoidance.

---

##  Tech Stack & Tools
* **OS:** Ubuntu 22.04 LTS (WSL 2)
* **ROS Version:** ROS 2 Humble
* **Simulation:** Gazebo Classic / Ignition Gazebo & RViz2
* **Language:** C++, Python, XML/Xacro

---

##  Installation & Build

```bash
# Clone the repository
cd ~/mobile_robot/src
git clone git@github.com:mubashir-robotics/articulated-mobile-robot-ros2.git .

# Build the workspace
cd ~/mobile_robot
colcon build --symlink-install

# Source the workspace
source install/setup.bash
```
---
## Launching the Robot

```bash
ros2 launch my_robot rsp.launch.py
```
