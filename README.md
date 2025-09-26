# roboticsapplications
# Robotics Applications Course

A hands-on course introducing robotics software, hardware, and reinforcement learning using **ROS 2**, **TurtleBot**, and **simulation environments**. Students progress from fundamental concepts to practical robot applications and advanced reinforcement learning for robotics.

---

## Prerequisites

Before starting, you should be familiar with:

- **C++**: Classes, inheritance, compiling, building with `cmake`  
- **Python**: Functions, NumPy, matplotlib  
- **Linux fundamentals**: File system, bash commands, package management, ssh  
- **Reinforcement Learning basics**: Policies, value functions, PPO algorithm  

---

##  Course Structure

### Module 1: ROS 2 Basics
**Concepts**
- Introduction to ROS 2 concepts: nodes, topics, services, parameters  
- Creating workspaces, building packages (`colcon build`), launching nodes  
- Writing publishers and subscribers in C++ and Python  

**Assignment 1: Build Two ROS 2 Nodes Exchanging Information**  
- Publisher node sends a number (e.g., counter).  
- Subscriber node receives it, processes it (e.g., square), and logs the result.  
- *Outcome*: Understand ROS 2 pub/sub communication.  

**Assignment 2: Build a Mobile Robot Model in URDF and Teleoperate It**  
- Create a differential-drive robot URDF (base + wheels + lidar/camera).  
- Visualize in RViz and simulate in Gazebo.  
- Drive using `teleop_twist_keyboard` or joystick.  
- *Outcome*: Learn URDF modeling and robot simulation basics.  

---

### Module 2: TurtleBot Applications
**Concepts**
- Introduction to TurtleBot3 (simulation & hardware setup)  
- Using TurtleBot navigation stack (SLAM, planners, `move_base` / Nav2)  

**Assignment 3: Integrate a Global or Local Planner**  
- Choose a planner (A*, Dijkstra, DWA, or TEB).  
- Configure it in TurtleBot’s navigation stack.  
- Test in simulation and on a real TurtleBot.  
- *Outcome*: Experience practical robot navigation — path planning, obstacle avoidance, and execution.  

---

### Module 3: Architecture & Hardware

**Assignment 4: Design a Class Architecture in C++**  
- Given a robotics problem (e.g., “a robot control system”), design classes such as `Sensor`, `Controller`, `Actuator`.  
- Implement interactions showing the flow of control.  
- *Outcome*: Practice modular design and understand robotics software layers.  

**Assignment 5: Write a Driver Using Datasheet Values**  
- Select a hardware component (e.g., IMU, motor driver).  
- Extract 2–3 key parameters from its datasheet.  
- Implement a simple driver in C++ or Python that reads/simulates those values.  
-  *Outcome*: Bridge low-level hardware datasheets to functional drivers.  

---

### Module 4: Reinforcement Learning for Robotics

**Concepts**
- Introduction to Gymnasium and Safety Gym  
- PPO (Proximal Policy Optimization) basics and workflow  

**Assignment 6: Run PPO on a Safety Hopper Environment**  
- Train a PPO agent in Gymnasium’s Safety Hopper.  
- Record reward curves and constraint violations.  
-  *Outcome*: Run baseline RL experiments in simulation.  

**Assignment 7: RL-Based Simulation on TurtleBot**  
- Train a TurtleBot in simulation with PPO, DQN, or SAC.  
- Task: goal reaching or obstacle avoidance.  
- Compare with classical planning.  
-  *Outcome*: Compare learning-based vs. model-based planning.  

---

### Module 5: Perception

**Assignment 8: Build a 2D Occupancy Grid from LiDAR Data**  
- Input: LiDAR scan as `(angle_deg, range_m)` pairs.  
- Mark cells along rays as free, endpoints as occupied.  
- Store grid in NumPy and visualize with matplotlib (`imshow`).  
-  *Outcome*: Learn how LiDAR data is transformed into occupancy grids for mapping/navigation.  

---
