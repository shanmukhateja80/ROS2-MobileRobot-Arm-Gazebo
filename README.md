# 🚀 ROS2 Mobile Robot + 2-DOF Arm

**(URDF | Gazebo | RViz | TF | ROS2 Jazzy)**

## 📌 Overview

This project demonstrates the design, simulation, and integration of a custom mobile robot equipped with a 2-DOF robotic arm using ROS2 Jazzy.

The goal of this project was to build a fully functional robot model from scratch — including kinematics, dynamics, control plugins, and visualization — and integrate all components into a cohesive ROS2 system.

---

## 🧠 System Architecture

The robot consists of:

* 🔹 Differential-drive mobile base
* 🔹 2-DOF robotic arm mounted on the base
* 🔹 Camera sensor plugin
* 🔹 TF tree connecting all links
* 🔹 Gazebo simulation with physics & controllers
* 🔹 RViz visualization

All subsystems run simultaneously under ROS2.

---

## 🔧 Features Implemented

### 🔹 Robot Modeling

* Custom URDF/Xacro modeling
* Proper link inertias & collision geometry
* Joint limits and dynamics configuration
* Modular Xacro structure

### 🔹 Mobile Base

* Differential drive Gazebo plugin
* Velocity command interface
* `/cmd_vel` topic integration

### 🔹 2-DOF Robotic Arm

* Joint position controllers
* Configured limits and dynamics
* Position command publishing

### 🔹 Simulation (Gazebo)

* Physics-enabled robot simulation
* Controller plugins integration
* Camera sensor plugin

### 🔹 Visualization (RViz)

* TF tree visualization
* Robot model rendering
* Live camera feed
* Joint state monitoring

---

## 📊 Concepts Demonstrated

* URDF & Xacro modeling
* TF tree management
* Gazebo plugin integration
* Joint controllers
* Differential drive kinematics
* Multi-component robot integration
* ROS2 topic-based control architecture

---

## ▶ How to Run

### 1️⃣ Build Workspace

```bash
colcon build
source install/setup.bash
```

### 2️⃣ Launch Gazebo Simulation

```bash
ros2 launch mobile_robot_description gazebo.launch.py
```

### 3️⃣ Launch RViz

```bash
ros2 launch mobile_robot_description display.launch.py
```

### 4️⃣ Teleoperate Mobile Base

```bash
ros2 run mobile_robot_control teleop_control.py
```





ing this strategically.
