---
layout: project
title: YooHoo! Guard — Child Safety Wearable (Senior Design Project)
date: 2025-12-01
description: Led system integration and product development for a multi-sensor child safety wearable that unifies water-risk detection, location tracking, biometric monitoring, and sleep-posture awareness into a single, age-adaptive platform.
technologies: [Systems Engineering, Wearable Devices, Sensor Fusion, DFMEA, CAD, Mechatronics, Product Design]
image: /assets/images/yoohoo/wb.gif
hero_image: /assets/images/yoohoo/v.gif
---

## Project Overview
**YooHoo! Guard** is a senior design capstone project focused on developing a **multi-functional child safety wearable** that provides continuous, real-time monitoring across multiple high-risk scenarios using a single, unified device. The project addresses a key gap in existing child-safety solutions, which are typically fragmented, single-purpose, and quickly become obsolete as children grow.

The system integrates **water-risk detection, location tracking with geofencing, physiological monitoring, and infant sleep-posture detection** into a compact wearable that adapts from infancy through early childhood. The final design reached a **prototype-ready, feasibility-validated stage**, supported by detailed CAD, system architecture, DFMEA, sustainability analysis, and a complete business case.

<figure style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/yoohoo/core.png' | relative_url }}"
       alt="YooHoo Guard system overview"
       style="width: 900px; max-width: 100%; height: auto; display: block; margin: 0 auto; border-radius: 14px; box-shadow: 0 8px 18px rgba(0,0,0,.12);">
</figure>


## System Architecture & Core Functions
YooHoo! Guard integrates four sensing subsystems into a **single safety engine**, with onboard logic that validates events across modalities to reduce false alarms:

- **Water-risk detection** using pressure-based depth sensing  
- **Location tracking & geofencing** via GNSS and LTE-M connectivity  
- **Physiological monitoring** (heart rate and SpO₂) using optical sensing  
- **Motion & sleep-posture detection** using an IMU  

All sensor streams are fused through microcontroller-based safety logic that filters noise, cross-validates events, and triggers alerts only when verified hazard conditions are detected. Alerts are delivered within **≤ 3 seconds** using redundant channels (mobile app + SMS fallback).
<div class="carousel">
  <button class="carousel-btn prev" aria-label="Previous image">&#10094;</button>
  <div class="carousel-track">
    <img src="{{ '/assets/images/yoohoo/block.png' | relative_url }}" alt="Infant clip configuration" class="carousel-img active">
    <img src="{{ '/assets/images/yoohoo/block-diagram.png' | relative_url }}" alt="Wristband configuration" class="carousel-img">
  </div>
  <button class="carousel-btn next" aria-label="Next image">&#10095;</button>
</div>


## Mechanical Design & Wearability
The device is built around a **sealed 40 mm × 10 mm electronics puck**, exceeding pediatric anti-choking thresholds while remaining comfortable for extended wear. A defining feature of the design is its **dual-mount, grow-with-the-child platform**:

- **Infant Mode:** snap-fit clothing attachment with a child-resistant push-and-turn release  
- **Child Mode:** wrist-worn configuration using a soft silicone band  

Material selection prioritized **safety, durability, and sustainability**, including PETG for the housing, TPU for edge interfaces, silicone gaskets for waterproofing, and a polycarbonate optical window. Rounded geometry and controlled attachment forces ensure comfort while preventing accidental detachment. :contentReference[oaicite:2]{index=2}

<figure style="text-align: center; margin: 1.5rem 0;">
  <img
    src="{{ '/assets/images/yoohoo/yoo.gif' | relative_url }}"
    alt="YooHoo Guard system overview"
    style="width: 900px; max-width: 100%; height: auto; display: block; margin: 0 auto; border-radius: 14px; box-shadow: 0 8px 18px rgba(0,0,0,.12);"
  >
</figure>

## Safety Engineering & DFMEA
Safety-critical design decisions were driven by **Voice of Customer (VOC)** research, translated into engineering specifications using a **House of Quality (HoQ)**, and validated through repeated **Design Failure Mode and Effects Analysis (DFMEA)** cycles.

High-risk failure modes identified and mitigated included:
- Water ingress
- False alarms and missed detections  
- Sensor misclassification (motion and posture)  
- Clip detachment and choking risk  

Mitigations included vented pressure sensing with hydrophobic membranes, sensor-fusion logic, mechanical redesign of attachment interfaces, and redundancy in alert delivery.


## Electronics & Sensing Integration
Key hardware elements included:
- **Pressure sensing:** vented MEMS sensor enabling ≤ 13 cm depth resolution under immersion  
- **Location & connectivity:** Nordic nRF9160 SiP with LTE-M/NB-IoT and GNSS  
- **Biometrics:** MAX30102 optical sensor for SpO₂ and heart rate monitoring  
- **Motion sensing:** IMU-based posture and abnormal motion detection  

The architecture supports submersion up to **2 m for 1 hour**, global location tracking with **≤ 10 m accuracy**, and multi-day battery life through low-power system design.

## YooHoo! Guard Parent Mobile App

<figure style="text-align: center; margin: 1.5rem 0;">
  <img
    src="{{ '/assets/images/yoohoo/app.png' | relative_url }}"
    alt="YooHoo Guard system overview"
    style="width: 900px; max-width: 100%; height: auto; display: block; margin: 0 auto; border-radius: 14px; box-shadow: 0 8px 18px rgba(0,0,0,.12);"
  >
</figure>

## Sustainability & Lifecycle Design
A key innovation of YooHoo! Guard is its **modular lifecycle strategy**. The sealed electronics core is reused across developmental stages, while only low-impact mechanical components are replaced as needed. Life-cycle analysis showed:

- ~**83% lower total environmental impact** compared to a reference Apple Watch
- Manufacturing as the dominant impact stage (~98%), minimized through reduced material mass  
- Reduced electronic waste through reuse of PCB, sensors, and battery  

This approach balances child safety, long-term usability, and environmental responsibility.

<figure style="text-align: center; margin: 1.5rem 0;">
  <img
    src="{{ '/assets/images/yoohoo/impact.png' | relative_url }}"
    alt="YooHoo Guard system overview"
    style="width: 900px; max-width: 100%; height: auto; display: block; margin: 0 auto; border-radius: 14px; box-shadow: 0 8px 18px rgba(0,0,0,.12);"
  >
</figure>


## Team & Leadership
This project was completed by a five-person interdisciplinary team. My role focused on **product development and system integration**, including:

- Translating VOC and HoQ outputs into system architecture  
- Sensor selection and placement strategy  
- CAD development and enclosure design  
- Safety analysis and DFMEA iteration  
- Coordination across technical and business subteams  

The project was mentored by Cornell faculty and Johnson School MBA advisors, combining rigorous engineering design with market and startup strategy.


## Engineering Takeaways
YooHoo! Guard demonstrated that effective safety wearables require systems-level thinking, where mechanical design, sensing, software logic, user behavior, and sustainability are tightly coupled. The project reinforced the importance of **designing for reliability and trust**, especially when engineering decisions directly affect child safety.


## Impact
- Unified four major child-safety functions into a single wearable platform  
- Delivered a prototype-ready, DFMEA-validated system architecture  
- Demonstrated age-adaptive, sustainable wearable design  
- Established a strong foundation for future prototyping and commercialization
