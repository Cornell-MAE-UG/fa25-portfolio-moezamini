---
layout: project
title: Water Screen Display — Programmable Droplet Projection
date: 2024-10-01
description: Designed and built a programmable water screen capable of rendering 2D objects using precisely controlled falling water droplets driven by solenoid valves and a Raspberry Pi.
technologies: [Embedded Systems, Mechatronics, Raspberry Pi, Power Electronics, Fluid Mechanics, Solenoid Control, Real-Time Control]
image: /assets/images/WS/w3.png
hero_image: /assets/images/WS/w3.png
---

## Project Overview
This project involved the design and construction of a **programmable water screen display** capable of visualizing **2D shapes and patterns** using falling water droplets. By precisely controlling the timing of individual droplets, the system creates the illusion of static images and dynamic patterns as water falls through free space.

The system combined **embedded control, power electronics, and mechanical design**, transforming a traditionally analog medium—water—into a digitally addressable display.

<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/WS/w5.png' | relative_url }}"
       alt="Water screen display overview"
       style="width: 600px; max-width: 100%; height: auto; display: block; margin: 0 auto;">
</figure>

---

## System Architecture
The water screen consisted of **23 independently controlled miniature solenoid valves**, each acting as a single vertical “pixel” in the display.

Core subsystems included:
- **Raspberry Pi** for high-level control and pattern generation  
- **MOSFET driver circuitry** to safely switch solenoid valves  
- **Solenoid valve array** controlling discrete water streams  
- **Gravity-driven droplet formation** for visual pattern rendering  
- **A mini Water Pump** for circulating water up to soleniod valves  

Each valve was switched with precise timing to determine when droplets were released, allowing spatial patterns to emerge as the water fell.

The mechanical structure was laser-cut from acrylic sheets and assembled using silicone sealant to ensure structural integrity and water-tight sealing throughout the system.

<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/WS/w6.png' | relative_url }}"
       alt="Water screen display overview"
       style="width: 600px; max-width: 100%; height: auto; display: block; margin: 0 auto;">
</figure>
---

## Droplet Timing & Pattern Generation
Visual patterns were created by mapping **2D binary images** into time-domain valve control signals.

Key implementation details:
- Each column of the image corresponded to one solenoid valve  
- Rows of the image were converted into timed valve-open pulses  
- Droplet spacing and image aspect ratio were tuned via pulse width and timing offsets  
- Synchronization across all 23 channels ensured coherent pattern formation  

This approach converted spatial information into **temporal control**, a core challenge of the project.

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/WS/w1.gif' | relative_url }}" alt="Droplet timing visualization" class="carousel-img active">
    <img src="{{ '/assets/images/WS/w2.png' | relative_url }}" alt="Valve array" class="carousel-img">
    <img src="{{ '/assets/images/WS/w4.png' | relative_url }}" alt="Pattern projection" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

---

## Electronics & Control
Each solenoid valve was driven through a **MOSFET-based switching stage**, allowing the low-power Raspberry Pi GPIO pins to safely control inductive loads.

Design considerations included:
- Flyback diode protection for inductive switching  
- Power isolation between logic and valve supply  
- Reliable high-speed switching across multiple channels  
- Modular wiring for easy debugging and expansion  

The electronics were designed for robustness and repeatability during extended operation.

---

## Engineering Takeaways and Challenges
This project demonstrated how precise timing control can be leveraged to create spatial and visual effects using discrete fluid droplets. Translating visual patterns into accurate droplet timing required careful consideration of fluid behavior, gravity, surface tension, and the response times of electromechanical components.

The project served as a hands-on exploration of system integration, reinforcing how software timing, electrical switching, and mechanical dynamics must be treated as a tightly coupled system. One of the primary challenges was synchronizing electrical actuation with fluid droplet formation and mechanical response, which required iterative testing and refinement. These challenges significantly deepened my understanding of precision timing, fluid dynamics at small scales, and electromechanical coordination.
