---
layout: project
title: Cube Craze Autonomous Robot — “Black Pearl”
date: 2025-05-01
description: Designed and built the fastest autonomous robot in Cornell’s 2026 Cube Craze competition, optimized for high-speed cube collection under strict budget and component constraints.
technologies: [Autonomous Robotics, Embedded Systems, Power Electronics, Sensor Fusion, Rapid Prototyping, Mechanical Design]
image: /assets/images/robot/C-cover.png
hero_image: /assets/images/robot/C9.gif
---
## Project Overview
This autonomous robot was developed for the MAE 3780: Mechatronics cube craze competition at Cornell University in Spring 2025. The objective was to collect as many cubes as possible within a constrained arena. Our team designed a pirate‑themed robot named Black Pearl, engineered for rapid cube acquisition and reliable retention under strict constraints on budget, components, geometry, and timeline.

This project was completed in collaboration with two classmates within two weeks. Our design philosophy emphasized speed, high drivetrain performance, and robust boundary detection. These priorities resulted in the fastest robot in the competition, supported by one of the most reliable maneuvering algorithms we developed for this project. 

<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/robot/C6.png' | relative_url }}"
       alt="Cube Craze robot overview"
       style="width: 600px; max-width: 100%; height: auto; display: block; margin: 0 auto;">
</figure>

---

## Drivetrain Optimization
To maximize robot speed within electrical constraints, we integrated a boost DC–DC converter to step the available 6 V supply up to 24 V, significantly increasing motor speed and drivetrain output. This approach provided a substantial performance advantage over competing robots by enabling faster traversal of the arena, earlier access to cubes, and higher overall collection rates.

Careful tuning ensured that the motors operated within safe current limits while achieving maximum usable RPM, balancing speed, reliability, and electrical robustness.

---

## Intake & Cube Retention System
The cube capture mechanism was intentionally designed to be ultra-lightweight and mechanically simple, reflecting our primary goal of maximizing speed and drivetrain performance. To minimize system mass, the intake structure and cube containment enclosure were fabricated from rigid poster board, providing sufficient stiffness while keeping inertia low.

A passive one-way intake door was implemented using a hinged mechanism that allowed cubes to enter the enclosure while preventing them from escaping once captured. This design enabled reliable retention without additional actuators or control complexity.

Key design features included:

- A passive one-way intake door for reliable cube capture

- Side-wall geometry that guided cubes inward during high-speed motion

- Lightweight construction using poster board to minimize mass and inertia

- No reliance on additional motors, sensors, or complex linkages

This minimalist approach reduced potential failure points, improved acceleration, and ensured consistent cube retention even during aggressive maneuvers at high speeds.

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/robot/C5.png' | relative_url }}" alt="Intake mechanism" class="carousel-img active">
    <img src="{{ '/assets/images/robot/C1.jpeg' | relative_url }}" alt="Cube capture system" class="carousel-img">
    <img src="{{ '/assets/images/robot/C3.png' | relative_url }}" alt="Side wall geometry" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

---

## Sensing & Navigation
Autonomous navigation was achieved using **dual QTI sensors** combined with a **custom filtering algorithm** to robustly detect field boundaries.

System capabilities included:
- Reliable boundary detection under variable lighting  
- Noise rejection through software filtering  
- Execution of a **diamond-shaped navigation path** optimized for cube interception  

The sensing logic enabled consistent, repeatable motion without reliance on complex localization or mapping.

<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/robot/C7.png' | relative_url }}"
       alt="QTI sensor placement"
       style="width: 1000px; max-width: 100%; height: auto; display: block; margin: 0 auto;">
</figure>
<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/robot/C8.png' | relative_url }}"
       alt="QTI sensor placement"
       style="width: 600px; max-width: 100%; height: auto; display: block; margin: 0 auto;">
</figure>
---

## Engineering Takeaways
This project reinforced that in highly constrained robotics competitions, goal-oriented decision-making and strategic simplicity often outperform system complexity. Rather than pursuing elaborate mechanisms or sensing architectures, performance was driven by focused optimization of the factors that mattered most to the competition objective.

Key contributors to success included strategic power management, aggressive mass reduction, and robust minimal sensing. Together, these choices demonstrated how performance can emerge from disciplined engineering tradeoffs rather than added complexity.

Black Pearl validated the importance of systems-level optimization, where electrical, mechanical, and algorithmic decisions are tightly coupled and aligned with a single, well-defined goal. This approach enabled a simple autonomous system to outperform significantly more complex robots in the field.

---

## Impact
- Achieved high-speed autonomous operation under strict constraints  
- Demonstrated effective power electronics integration for performance gains  
- Delivered a robust, low-complexity solution with minimal failure points
- Implemented a custom, goal-oriented autonomous control algorithm
