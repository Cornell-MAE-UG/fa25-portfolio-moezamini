---
layout: project
title: Braking System of Mag-lev pod— Cornell Hyperloop
date: 2025-04-01
description: Led the braking subsystem for Cornell Hyperloop, designing and validating redundant pneumatic and magnetic braking systems to ensure safe, reliable full-stop capability under competition constraints.
technologies:   [  Mechanical System Design,
  Material Selection,
  Electromechanical Systems,
  Pneumatic Actuation,
  Magnetic Systems,
  Safety-Critical Engineering,
  DFMEA,
  Automation & Controls,
  FEA,
  Prototyping,
  Experimental Testing & Validation,
  GD&T,
  Machining & Manufacturing
]
image: /assets/images/hyperloop/hyperloop-card.png
hero_image: /assets/images/hyperloop/H8.png
---

<h2 style="display: flex; align-items: center; gap: 12px;">
  Cornell Hyperloop
  <img src="{{ '/assets/images/logo/hyperloop-logo.png' | relative_url }}"
       alt="Cornell Hyperloop logo"
       style="height: 36px; width: auto;">
</h2>

<a href="https://www.cornellhyperloop.com/">Cornell Hyperloop</a> is a student-led engineering project team at <a href="https://www.cornell.edu/">Cornell University</a> that designs and builds high-speed magnetic levitation pods for hyperloop transportation; a revolutionary system where pods travel through vacuum-sealed tubes at hundreds of miles per hour. With 60+ members across Mechanical, Electrical/Software, and Business teams, we're advised by Cornell faculty <a href="https://www.engineering.cornell.edu/people/zhiting-tian/" style="text-decoration: underline;">Professor Zhiting Tian</a> and <a href="https://economics.cornell.edu/rick-geddes" style="text-decoration: underline;">Professor Rick Geddes</a>.
We compete annually in May at the Canadian Global Hyperloop Competition at the <a href="https://uwaterloo.ca/">University of Waterloo</a>. Cornell Hyperloop previously competed in the <a href="https://www.boringcompany.com/hyperloop">SpaceX Hyperloop Competition</a>.


## Braking Subteam Overview
As Braking Team Lead for the Cornell Hyperloop Project Team, I led the design, fabrication, integration, and testing of safety-critical braking systems for a Hyperloop maglev pod across multiple project cycles and competitions. The braking subsystem was required to reliably bring the pod to a full stop under both nominal and failure conditions while meeting strict constraints on mass, cost, manufacturability at the university machine shop, and competition compliance.
My responsibilities spanned leadership, project organization, system architecture, mechanical and magnetic design, automation logic, and experimental validation. I coordinated closely with propulsion, structures, and controls subteams, and authored the braking system user manual for competition submission.

Our pod employs two complementary braking systems:

- **Magnetic braking:** A customized Halbach array with on/off capability serves as the primary braking system, smoothly decelerating the pod from extreme high speeds without damaging the track

- **Frictional braking:** A pressurized air and pneumatic cylinder system provides full-stop capability and serves as the emergency braking system in cases of power failure or disruption in the magnetic braking system

---

## Braking System Architecture
The braking strategy employed multiple, independent mechanisms to ensure fail-safe operation:

- **Primary magnetic braking** for non-contact rapid deceleration and energy efeciency  
- **Pneumatically actuated frictional brakes** for guaranteed full-stop capability  
- **Automated failover logic** to engage emergency braking (frictional braking) during power loss or magnetic brake failure

This layered approach ensured compliance with Hyperloop safety requirements while maintaining robustness under uncertain operating conditions.

---

## Pneumatic Emergency Braking
I designed, built, and tested a pneumatically actuated frictional braking system capable of reliably stopping the pod and engaging automatically in the event of primary system failure.

Key engineering considerations included:
- Rapid actuation and consistent braking force  
- Mechanical robustness under dynamic loading  
- Integration with onboard air supply and control valves  
- Fail-safe behavior during electrical power loss  

The system was fully automated to default to braking when power is removed, providing intrinsic safety through mechanical and pneumatic design rather than software dependence.

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/hyperloop/H9.png' | relative_url }}" alt="Pneumatic brake assembly" class="carousel-img active">
    <img src="{{ '/assets/images/hyperloop/H4.png' | relative_url }}" alt="Emergency brake deployment" class="carousel-img">
    <img src="{{ '/assets/images/hyperloop/H13.png' | relative_url }}" alt="Pneumatic brake testing" class="carousel-img">
    <img src="{{ '/assets/images/hyperloop/H03.png' | relative_url }}" alt="Pneumatic brake testing" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

---

## Magnetic Braking & Halbach Array Development
In parallel, I researched and prototyped an advanced magnetic braking system based on a novel circular Halbach array design to generate strong, localized magnetic fields for contactless braking. The customized architecture enables effective on/off control of permanent magnets through a simple 30-degree mechanical rotation, enabling:

- High braking force when engaged

- Near-complete magnetic field shielding when disengaged

- Significant reduction of stray magnetic flux near sensitive subsystems, minimizing electromagnetic interference, improving transport safety, and enabling precise control of magnetic field exposure

Design highlights included:

- Optimization of magnet orientation to maximize braking force

- Modular construction to support rapid iteration

- Mechanical simplicity compatible with student fabrication capabilities

This work explored scalable magnetic braking concepts relevant to high-speed maglev systems.

<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/hyperloop/H10.png' | relative_url }}" alt="magnetic brake assembly" class="carousel-img active">
    <img src="{{ '/assets/images/hyperloop/H16.png' | relative_url }}" alt="magnets" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>

---

## Automation & Failure Handling
I implemented braking automation logic from the ground up to continuously monitor system health and trigger emergency braking under fault conditions.
Failure modes addressed included:
- Electrical power loss  
- Magnetic braking system malfunction  
- Command or communication failure  

By designing the system to fail into a safe state, the braking subsystem maintained reliability independent of higher-level control software.

---

## Engineering Leadership
As Braking Team Lead, I:

- Defined subsystem requirements and safety constraints

- Managed timelines, design reviews, and documentation

- Trained and mentored new team members

- Coordinated interfaces with propulsion, structures, and controls teams

- Balanced performance, safety, and manufacturability tradeoffs

This role required both technical depth and systems-level leadership in a multidisciplinary engineering environment.

---

## Engineering Takeaways
This project reinforced the importance of redundancy, simplicity, and fail-safe design in safety-critical systems. Effective braking performance depended not only on analytical force calculations, but on robust actuation, reliable interfaces, and clear failure-handling strategies under real-world conditions.

Leading the braking subsystem provided hands-on experience designing, machining, assembling, and testing hardware where engineering decisions have immediate safety implications.

---

## Impact
- Delivered a redundant braking architecture with automated fail-safe behavior  
- Enabled reliable full-stop capability under nominal and failure conditions  
- Advanced magnetic braking concepts for future Hyperloop iterations  
- Strengthened system safety, compliance, and manufacturability
