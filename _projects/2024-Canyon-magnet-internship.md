---
layout: project
title: Canyon Magnet Energy — HTS Flux Pump Development
date: 2024-08-01
description: Researched, designed, and fabricated a dynamo-type high-temperature superconducting (HTS) flux pump delivering up to 700 A into superconducting magnet coils under cryogenic conditions.
technologies: [HTS Magnets, Cryogenics, Electromechanical Design, Superconductivity, Coil Winding, Prototyping, Testing]
image: /assets/images/canyon/B2.png
hero_image: /assets/images/canyon/B2.png
---

## Project Overview
At **Canyon Magnet Energy**, I led the development of a **dynamo-type High-Temperature Superconducting (HTS) flux pump** designed to inject large persistent currents into superconducting magnet coils without direct electrical contact. This work was completed as part of a **Summer 2024 engineering internship**.

The project operated at the intersection of **electromechanical system design, cryogenics, and superconducting physics**, with the objective of achieving stable, high-current operation at **liquid nitrogen temperatures (77 K)**. I held end-to-end design ownership of the system, guiding the project from initial research and concept development through DFMEA, mechanical and electrical design, fabrication, and experimental validation.

---

## HTS Flux Pump Design
Flux pumping is a technique used to magnetize superconducting coils by inducing current through time-varying magnetic fields, eliminating the need for direct electrical connections. This approach reduces power losses and enables persistent-current operation in high-field superconducting magnets, where relatively low injected currents accumulate over time to produce very large circulating currents within the superconducting coil.

Two primary flux pump architectures exist in the literature:
- **Dynamo-type flux pumps**, which use rotating permanent magnets to induce current in superconducting tape  
- **Transformer–rectifier flux pumps**, which rely on magnetic coupling and rectification techniques  

For this project, I selected and custom-designed a **dynamo-type HTS flux pump**, as it offered greater mechanical simplicity, lower cost, and better alignment with the project’s experimental goals compared to transformer–rectifier approaches.

The system was designed to deliver up to **700 A** into superconducting magnet coils under cryogenic conditions. Key design elements included permanent magnet rotors, mechanical synchronization mechanisms, and parallel-wired HTS tape configured into a **double-pancake coil geometry**.

Key technical aspects included:
- Non-contact current injection into HTS coils  
- Mechanical synchronization of rotating magnetic elements  
- Stable operation at **77 K** using liquid nitrogen cooling  
- Compatibility with multiple HTS tape geometries and coil configurations  


<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/canyon/B3.gif' | relative_url }}" alt="cryo-box with dynamo typ assy" class="carousel-img active">
    <img src="{{ '/assets/images/canyon/B8.png' | relative_url }}" alt="Transformer rectifier CAD" class="carousel-img">
    <img src="{{ '/assets/images/canyon/B2.png' | relative_url }}" alt="Dynamo type" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>
---

## Cryogenic Test Infrastructure
To support controlled testing of HTS coils and flux pump performance, I designed and fabricated a **custom liquid nitrogen cryogenic test enclosure**.

Key design considerations included:
- Thermal insulation and controlled nitrogen boil-off  
- Secure mechanical fixturing for HTS coils and rotating components  
- Safe handling procedures and repeatable cooldown cycles  
- Optical and electrical access for diagnostics and instrumentation  
- Integration of pressure-relief features and cryogenic-compatible materials  
- Electrical safety considerations for high-current operation  

This test infrastructure enabled reliable evaluation of current injection performance and superconducting behavior under realistic operating conditions.

---

## Engineering Takeaways
This project highlighted the strong coupling between **mechanical design, electromagnetic behavior, and thermal constraints** in superconducting systems operating under extreme conditions. Taking ownership of a complex, novel system from inception reinforced a structured approach to tackling open-ended engineering problems through iterative design, risk analysis, and experimentation.

Working within a startup research environment emphasized the importance of **rapid prototyping, experimental validation, and cross-disciplinary engineering judgment** when pushing performance boundaries at the edge of current technological capabilities.
