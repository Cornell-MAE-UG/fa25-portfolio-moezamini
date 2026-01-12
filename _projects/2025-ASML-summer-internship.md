---
layout: project
title: ASML Mechanical Design Internship
date: 2025-08-01
description: Designed, tested, and validated precision mechanical systems for integrating optical transceivers into ASML lithography platforms, enabling nanometer-level alignment under extreme dynamic loading.
technologies: [Precision Mechanical Design, Optical Alignment, Tolerance Analysis, Test Fixtures, FEA, Vibration & Shock, Manufacturing]
image: /assets/images/asml/asml-cover.png
hero_image: /assets/images/asml/asml-card.png
---

## Project Overview
During my internship at **ASML**, I worked on the mechanical design, testing and system integration of **optical transceivers** used for high-speed data communication within the **reticle stage** of advanced photolithography systems, which operate under **extreme acceleration** while requiring **nanometer-level positional accuracy**.

My project centered on feasibility assessment as well as the design, testing, and validation of optical transcivers to ensure reliable optical performance under stringent alignment requirements, vibration, and shock loading. This work directly contributed to improving system robustness, manufacturability, and long-term reliability for next-generation lithography platforms.


<figure style="text-align: center; margin: 1.5rem 0;">
  <img 
       src="{{ '/assets/images/asml/a4.png' | relative_url }}"
       alt="ASML optical transceiver integration"
       style="width: 1000px; max-width: 100%; height: auto; display: block; margin: 0 auto; border-radius: 10px; box-shadow: 0 8px 16px rgba(0,0,0,0.18);">
</figure>

---

## System Context
The optical transceiver assemblies operate within a high-precision, high-acceleration environment characterized by:

- Extremely tight positional and angular tolerances

- High-frequency motion of the reticle stage

- Application to next-generation photolithography platforms operating at accelerations exceeding 40 G

- Strict cleanliness, materials, and reliability constraints

- Integration into ASML’s PFAS-reduction initiative, enabling the removal of PFAS-containing cabling from the system

- A requirement to reduce system cost and mass by at least 30% compared to the legacy design

Even small mechanical misalignments at the interface level can degrade signal integrity by increasing bit-error rates and timing skew — making mechanical design a first-order driver of optical performance.


---

## Precision Test Fixture Design
To evaluate optical performance under controlled misalignment conditions, I designed and validated a **4-degree-of-freedom (4-DOF) precision test fixture** capable of independently adjusting components with nanometer-scale precision in:

- Lateral translation  
- Vertical translation  
- Scan-direction translation  
- Angular pitch  

**Key characteristics of the fixture included:**

- **Nanometer-scale positional resolution**  
- **Milliradian-level angular control**  
- High mechanical stability under repeated test cycles  
- Full compatibility with optical signal-characterization workflows  
- Adaptability to multiple transceiver architectures  
- Internal shielding to minimize stray light noise  

**This fixture enabled systematic testing of:**

- Signal-strength degradation  
- Delay-skew sensitivity  
- Bit-error rate as a function of mechanical misalignment  

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/asml/a2.png' | relative_url }}" alt="Precision fixture CAD" class="carousel-img active">
    <img src="{{ '/assets/images/asml/a1.png' | relative_url }}" alt="Fixture alignment stages" class="carousel-img">
    <img src="{{ '/assets/images/asml/a3.png' | relative_url }}" alt="Optical testing setup" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

---

## Structural Design & Dynamic Validation

In parallel with the test fixture development, I designed and analyzed a **functional mounting architecture** for the transceiver assembly intended for in-system deployment.

**Engineering focus areas included:**

- Structural stiffness and load-path integrity under **43 g acceleration events** in next-generation photolithography systems  
- Alignment retention under shock and vibration loading  
- Tolerance stack-up analysis to preserve optical performance margins  
- Design for manufacturability and assembly repeatability  

Finite-element analysis and analytical hand calculations were used to evaluate deformation modes and verify that alignment errors remained within allowable optical limits under worst-case dynamic loading. Results from the precision test fixture — characterizing optical performance sensitivity to positional and angular misalignment, were incorporated into the structural design to ensure robust mounting of the transceivers to the reticle stage.

---

## Sustainability & Manufacturability Considerations
The final design contributed to broader system-level goals by:
- Supporting **PFAS-free material initiatives**  
- Reducing component complexity and cost  
- Improving long-term reliability through robust mechanical constraint  
- Enabling repeatable assembly without post-assembly optical tuning  

These considerations ensured that performance gains were achieved without compromising ASML’s manufacturing scale or sustainability targets.

---

## Key Takeaways

During my internship at **ASML**, I learned how to communicate and collaborate effectively within a large, multidisciplinary engineering organization. I became comfortable preparing for and contributing to professional technical meetings, and I gained firsthand experience in designing for manufacturability and cost reduction.

I also saw how reliability issues can propagate through complex systems, and how large engineering teams work together to diagnose and resolve them in a structured, professional way. Being surrounded by exceptionally talented engineers and seeing the sophistication of ASML’s machines helped me become more confident in proposing ideas and approaching highly complex technical challenges.

The internship also strengthened my ability to manage time and priorities under tight deadlines while coordinating with multiple internal teams and external suppliers across disciplines.

This project reinforced that in ultra-precision systems, mechanical design and optical performance are inseparable. Achieving reliable signal integrity required careful control of stiffness, tolerances, and dynamic response, not just nominal geometry.

The work closely reflected real-world high-tech product development, where design choices must simultaneously satisfy performance, reliability, manufacturability, and sustainability requirements.


---

## Impact
- Enabled nanometer-level optical alignment under extreme acceleration  
- Delivered a validated 4-DOF precision test platform for optical characterization  
- Improved confidence in transceiver robustness during dynamic operation  
- Contributed to cost reduction and sustainability goals in advanced lithography systems
