---
layout: project
title: Cyclo Rotor — Multi-Environment Propulsion System
date: 2023-12-01
description: Researched, designed, and prototyped a cyclo-rotor propulsion system for a next-generation drone enabling operation across air, water, and ground environments.
technologies: [Aerodynamics, Rotorcraft Design, Electromechanical Systems, Prototyping, Robotics, Multiphysics Design]
image: /assets/images/cyclo/E7.png
hero_image: /assets/images/cyclo/E1.jpeg
---

## Project Overview
This project focused on the research, design, and prototyping of a **cyclo-rotor propulsion system** for a futuristic, multi-environment drone platform. Unlike conventional propellers, a cyclo rotor generates thrust by cyclically pitching rotating blades, enabling **vectorable thrust control** independent of vehicle orientation.

The long-term objective of the project is to develop a **versatile propulsion architecture** that allows a single robotic platform to operate effectively **in air, on land, and in water**, supporting future applications in exploration, inspection, and autonomous robotics. The project is in very early stages and continues improvments are being done on it. 

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>

  <div class="carousel-track">
    <img src="{{ '/assets/images/cyclo/E3.png' | relative_url }}"
         alt="Cyclo-rotor CAD concept model"
         class="carousel-img active">

    <img src="{{ '/assets/images/cyclo/E4.png' | relative_url }}"
         alt="Cyclo-rotor blade pitch control mechanism"
         class="carousel-img">
  </div>

  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

<p style="text-align: center; font-size: 0.9rem; opacity: 0.75; margin-top: 0.5rem;">
  Images adapted from:
  <a href="https://www.researchgate.net/publication/281121327_Development_of_Control_Strategies_and_Flight_Testing_of_a_Twin-Cyclocopter_in_Forward_Flight"
     target="_blank" rel="noopener">
    <em>Development of Control Strategies and Flight Testing of a Twin-Cyclocopter in Forward Flight</em>
  </a>
</p>

---

## Cyclo Rotor Concept
A cyclo rotor consists of multiple blades mounted around a rotating drum, where each blade’s **pitch angle is actively controlled** as it rotates. By adjusting blade pitch as a function of angular position, the rotor can produce thrust in arbitrary directions.

Key advantages explored in this project:
- Thrust vectoring without tilting the vehicle
- Rapid transition between lift and forward thrust
- Potential for improved maneuverability in confined spaces
- Applicability across different fluid environments  

This propulsion concept is particularly attractive for platforms requiring **high agility and environmental adaptability**.

---

## Mechanical Design & Prototyping
I designed and fabricated an initial cyclo-rotor prototype to validate mechanical feasibility and blade-pitch control concepts.

Engineering focus areas included:
- Rotor geometry, airfoil profile selection and blade mounting strategy  
- Pitch actuation mechanisms synchronized with rotor rotation  
- Structural stiffness and balance considerations  
- Manufacturability using rapid prototyping methods  

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/cyclo/E7.png' | relative_url }}" alt="Cyclo rotor CAD" class="carousel-img active">
    <img src="{{ '/assets/images/cyclo/E6.png' | relative_url }}" alt="Blade pitch mechanism" class="carousel-img">
    <img src="{{ '/assets/images/cyclo/E2.png' | relative_url }}" alt="Rotor assembly" class="carousel-img">
    <img src="{{ '/assets/images/cyclo/E1.jpeg' | relative_url }}" alt="Rotor assembly" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

---

## Control & Thrust Vectoring Strategy
A core technical challenge of cyclo-rotor systems is coordinating **blade pitch modulation** with rotor angular position.

Work in this area included:
- Developing conceptual pitch-angle profiles for thrust vectoring  
- Exploring mechanical versus electronic pitch control approaches  
- Evaluating control complexity versus achievable maneuverability  
- Identifying constraints imposed by actuator bandwidth and timing  

This aspect of the project remains ongoing, with continued efforts focused on refining control strategies and improving actuation feasibility.

---

## Multi-Environment Design Motivation
The cyclo rotor is being developed as part of a broader vision for **multi-modal robotic mobility**.

Design considerations included:
- Robustness to differing fluid densities (air vs. water)  
- Mechanical sealing and durability for amphibious operation  
- Compatibility with ground-based locomotion architectures  
- Scalability to different vehicle sizes  

Although still in an exploratory phase, the project establishes a foundation for future integrated prototypes.

---

## Engineering Takeaways
This project emphasized the value of **nontraditional propulsion concepts** in expanding the operational envelope of robotic systems. Cyclo-rotor designs require tight coupling between aerodynamics, mechanics, and control strategy, reinforcing the importance of systems-level thinking early in the design process.

Working on an unconventional architecture strengthened my ability to reason through open-ended, research-driven engineering problems where constraints are still evolving.



*Development on this project is ongoing, with future work focused on refining control strategies, improving mechanical robustness, and validating performance through experimentation.*