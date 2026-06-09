---
layout: project
title: "EPFL Xplore — Mars Rover"
description: "3 years building a Mars rover from scratch — structure, mechanical leadership, and ROS2 arm control. Winner ERC 2025."
date: 2022-09-01
categories: [Robotics]
tags: [ROS2, SolidWorks, 3D Printing, Computer Vision, Mechanical Design, PETG, TPU, MoveIt!]
featured_image: "/assets/images/projects/xplore/photo-01.jpg"
period: "Sep 2022 – Aug 2025"
organisation: "EPFL Xplore"
status: "Completed"
role: "Structure Engineer / Structure Team Lead / Robotic Arm Software"
team: "Multiple"
github_url: ""

# 3D Models - placeholder for later .glb
models:
  - file: "/assets/models/xplore-rover.glb"
    description: "EPFL Xplore Rover placeholder model (drop .glb at assets/models/xplore-rover.glb)"

# Photo gallery placeholders
gallery:
  - type: "image"
    file: "/assets/images/projects/xplore/photo-01.jpg"
    description: "Xplore Rover — overview"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-02.jpg"
    description: "Chassis and suspension"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-03.jpg"
    description: "Differential system and wheels"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-04.jpg"
    description: "Dual-material wheel printing"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-05.jpg"
    description: "Robotic arm integration"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-06.jpg"
    description: "Field testing"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-07.jpg"
    description: "Team photo"
  - type: "image"
    file: "/assets/images/projects/xplore/photo-08.jpg"
    description: "Competition highlights"

---

## Overview

I joined EPFL Xplore in 2022 and spent three years working across the full engineering stack — from hands-on mechanical fabrication to leading the structure team and building software pipelines. Each year the team builds a complete Mars rover from scratch to compete at the European Rover Challenge (ERC).

During my time I contributed mechanical designs, led the structure subsystem, and later moved into robotic arm software to unify control and perception pipelines.

---

## Year 1 — Structure Engineer (2022–2023)

- Contributed to rover design, prototyping and assembly.
- Designed and built the differential drive system.
- Fabricated wheels: 3D-printed inner rims and molds, cast PU coating for terrain grip.

**Result:** 🥉 3rd Place at ERC 2023 · 🏆 Maintenance Task Award

---

## Year 2 — Structure Team Lead (2023–2024)

- Led the structure subsystem team of 8 engineers.
- Worked on wheels, chassis and suspensions.
- Developed a dual-material wheel using a dual-extruder printer combining rigid PETG (structure) and flexible TPU (compliant elements) — improved damping on uneven terrain and reduced manufacturing time by ~50%.

**Result:** 🏆 Presentation Award 2024

---

## Year 3 — Robotic Arm Software Member (2024–2025)

- Joined the robotic arm software team, expanding from mechanical to software responsibilities.
- Implemented camera integration and vision-assisted grasp targeting for the arm.
- Semester project: "Implementing Multi-Modal Control for a Robotic Arm with ROS2 Control" — unified manual control, automatic inverse kinematics, velocity control, and torque-controlled gripper into a single ROS2 pipeline; validated in Gazebo + MoveIt!.
- Developed computer vision algorithms for drone obstacle detection used during competition.

**Result:** 🥇 1st Place ERC 2025 · 🏆 Excellence Award for Drone Navigation · 🏆 Innovation Prize

---

## Wheel Design — Technical highlight

| Specification | Details |
|--------------:|:--------|
| Structure material | PETG (rigid, lightweight) |
| Compliant elements | TPU (flexible, shock-absorbing) |
| Method | Dual-extruder 3D printing |
| Key benefit | Passive vibration damping + ~50% faster manufacturing vs previous design |

---

## ROS2 Pipeline — Technical highlight

| Item | Details |
|-----:|:--------|
| Framework | ROS2 |
| Simulation | Gazebo + MoveIt! |
| Control modes unified | Manual, Automatic IK, Velocity control, Torque-controlled gripper |
| Project type | EPFL Semester Project |

---

## 3D Model

<div class="project-model">
  <model-viewer src="{{ page.models.first.file | relative_url }}" alt="Xplore Rover 3D model" camera-controls auto-rotate style="width:100%; height:420px; background: transparent;">
  </model-viewer>
</div>

---

## Gallery

<div class="project-gallery">
  {% for item in page.gallery %}
    {% if item.type == "image" %}
      <img src="{{ item.file | relative_url }}" alt="{{ item.description }}" />
    {% endif %}
  {% endfor %}
</div>

---

## Awards & Recognition

- 🥇 1st Place, European Rover Challenge 2025
- 🏆 Excellence Award for Drone Navigation, ERC 2025
- 🏆 Innovation Prize, ERC 2025
- 🏆 Presentation Award, ERC 2024
- 🏆 Maintenance Task Award, ERC 2023
- 🥉 3rd Place, European Rover Challenge 2023

---

