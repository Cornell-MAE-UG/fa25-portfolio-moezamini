---
layout: project
title: Little Red Rover Autonomous Maze Navigation (Beta Test)
date: 2025-11-01
description: Implemented and evaluated autonomous navigation on the Little Red Rover platform using A* and RRT planners, particle-filter localization, and LiDAR-based sensing to enable reliable maze escape in ROS.
technologies: [ROS, Python, LiDAR, A*, RRT, Particle Filters, Sensor Fusion, Foxglove]
image: /assets/images/red_rover/t2.png
hero_image: /assets/images/red_rover/t2.png
---

## Project Overview
This project focused on autonomous navigation using the **Little Red Rover (LRR)** platform, a ROS-based educational robotics system. As part of the **LRR beta test**, I designed and validated a complete autonomy pipeline that enabled a Red Rover robot car to localize itself, plan collision-free paths, and successfully escape complex maze environments using onboard sensing.

The work emphasized **end-to-end autonomy and system integration**, rather than isolated algorithms, and required extensive debugging within a partially mature robotics software stack.


<figure style="text-align:center; margin: 1.25rem 0;">
  <img src="{{ '/assets/images/red_rover/pure_pursuit_demo.gif' | relative_url }}"
       alt="Little Red Rover system architecture"
       style="max-width:100%; height:auto; border-radius:10px;">
</figure>


## System Architecture Overview
The Little Red Rover platform is organized as a layered robotics system composed of four primary subsystems:

- **Hardware** — the physical rover platform, including motors, wheel encoders, IMU, and LiDAR sensors  
- **Firmware** — microcontroller-level software responsible for reading sensors and issuing low-level actuator commands  
- **ROS Drivers** — ROS nodes that bridge onboard firmware with the host computer, publishing sensor data and accepting motion commands  
- **Tooling** — cross-platform development and debugging tools supporting visualization and analysis (e.g., Foxglove)

Communication between these layers occurs through two key interconnects:
- **Hardware ↔ Firmware:** sensor acquisition and actuator control  
- **Firmware ↔ ROS:** transmission of state estimates, sensor data, and command messages  

My work focused primarily on the **ROS layer and system integration**, where localization, planning, and visualization interact with real sensor data and where most autonomy failures emerged during beta testing.

<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/red_rover/little_red_rover_system_diagram.svg' | relative_url }}"
       alt="Little Red Rover system architecture"
       style="width: 600px; max-width: 100%; height: auto; display: block; margin: 0 auto;">
</figure>



## Autonomous Planning
I implemented both **A\*** and **Rapidly-Exploring Random Tree (RRT)** planners in ROS to solve maze-navigation tasks.

Key contributions included:
- Designing planner pipelines capable of navigating narrow corridors, dead-ends, and cluttered environments  
- Comparing deterministic (A\*) and sampling-based (RRT) planning behavior under localization uncertainty  
- Tuning cost functions, step sizes, and goal tolerances to improve convergence reliability  
- Enabling the robot to **autonomously exit mazes without human intervention**

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/red_rover/maze.png' | relative_url }}" alt="rover image" class="carousel-img active">
    <img src="{{ '/assets/images/red_rover/r3.png' | relative_url }}" alt="rover image" class="carousel-img">
    <img src="{{ '/assets/images/red_rover/maze_demo.png' | relative_url }}" alt="rover image" class="carousel-img">
    <img src="{{ '/assets/images/red_rover/end.png' | relative_url }}" alt="rover image" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>


## Localization & Sensor Fusion
To support robust navigation, I implemented probabilistic localization using a **particle filter** that fused multiple onboard sensors:
- Wheel odometry  
- IMU measurements  
- LiDAR scan data  

I debugged transform (TF) chains, sensor alignment issues, and resampling logic to prevent particle depletion and localization divergence, particularly in long corridors and symmetric maze regions.


## ROS Integration & Visualization
I developed and debugged ROS launch files coordinating localization, planning, control, and visualization nodes.  
To accelerate debugging and validation, I used **Foxglove** to:
- Visualize LiDAR scans, particle distributions, and planned paths  
- Inspect TF trees and frame mismatches in real time  
- Diagnose planner failures and localization drift during execution  

This tooling enabled rapid iteration and system-level insight beyond basic simulation visualization.



## Engineering Takeaways
This project demonstrated that **autonomous navigation performance is driven by system integration rather than algorithms alone**. Minor issues such as TF inconsistencies, sensor noise, or resampling instability can fully undermine correct planning logic. Working within a beta-stage platform closely mirrored real-world robotics development, where debugging, observability, and iteration are core engineering skills.



## Impact
- Achieved fully autonomous maze escape using LiDAR-based perception  
- Gained hands-on experience with probabilistic localization in realistic conditions  
- Developed strong intuition for planning–localization coupling in mobile robots  
- Contributed informed feedback toward improving the Little Red Rover platform’s robustness and usability
