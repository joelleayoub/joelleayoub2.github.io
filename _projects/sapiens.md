---
layout: project
title: "SAPIENS Humanoid Robot"
description: "Leading development of EPFL's first humanoid robot (Mina) — full assembly, custom hand, wrist cameras, and an imitation learning pipeline."
date: 2026-02-01
categories: [Robotics]
tags: [ROS2, URDF, 3D Printing, Imitation Learning, MoveIt!, C++, Python]
featured_image: "/assets/images/projects/sapiens/photo-01.jpg"
status: "Active"
role: "Project Lead"
organisation: "EPFL AI Team"
team: "8 engineers"
period: "Feb 2026 – Present"
github_url: ""

# 3D Models - placeholder for later .glb
models:
  - file: "/assets/models/sapiens.glb"
    description: "SAPIENS placeholder model (drop .glb at assets/models/sapiens.glb)"

# Photo gallery placeholders
gallery:
  - type: "image"
    file: "/assets/images/projects/sapiens/photo-01.jpg"
    description: "SAPIENS — overview"
  - type: "image"
    file: "/assets/images/projects/sapiens/photo-02.jpg"
    description: "Assembly progress"
  - type: "image"
    file: "/assets/images/projects/sapiens/photo-03.jpg"
    description: "Custom hand prototype"
  - type: "image"
    file: "/assets/images/projects/sapiens/photo-04.jpg"
    description: "Wrist camera mount"
  - type: "image"
    file: "/assets/images/projects/sapiens/photo-05.jpg"
    description: "Team integration"
  - type: "image"
    file: "/assets/images/projects/sapiens/photo-06.jpg"
    description: "Testing and debugging"

components:
  - name: "Base Platform"
    quantity: 1
    description: "Berkeley Humanoid Lite (open-source)"
  - name: "Actuators"
    quantity: "Multiple"
    description: "Quasi-direct-drive motors, low gear ratio"
  - name: "Fabrication"
    quantity: "Many"
    description: "3D-printed structural components (PLA/PETG)"
  - name: "Perception"
    quantity: 2
    description: "Wrist-mounted cameras (custom mounts)"

---

## Project Overview

SAPIENS is EPFL's first full humanoid robot, developed within the EPFL AI Team. Based on the Berkeley Humanoid Lite open-source architecture, SAPIENS (Mina) is being developed to explore manipulation, perception, and integrated system design in a compact humanoid platform. I lead mechanics, software, and electronics development, manage budget and timeline, and coordinate the engineering team.

From hardware assembly and actuator integration to ROS2 software, URDF modelling, and the imitation learning pipeline, the project is a full-stack engineering effort aimed at rapid iteration and reproducible results.

## Short Description (project card)

Leading a team of 8 building EPFL's first humanoid robot based on Berkeley Humanoid Lite — full assembly, custom dexterous hand, wrist cameras integrated in URDF, and an imitation learning pipeline for manipulation.

## My Contributions

- Printed, iterated, and assembled the full humanoid platform, focusing on mechanical robustness and cable routing.
- Redesigned the dexterous hand for improved finger kinematics and manufacturability.
- Designed and integrated wrist-mounted camera supports (physical mounts and URDF inclusion).
- Coordinated system integration across mechanics, software, and electronics; managed timeline and procurement.
- Developed ROS2 interfaces, MoveIt! integration, and tools for demonstration collection for imitation learning.

## Technical Specifications

| Specification | Value |
|---------------|-------|
| **Base Platform** | Berkeley Humanoid Lite (open-source) |
| **Actuation** | Quasi-direct-drive motors, low gear ratio |
| **Fabrication** | 3D-printed structural components (PLA/PETG) |
| **Perception** | Wrist-mounted cameras (custom mounts) |
| **Software Stack** | ROS2, MoveIt!, Python/C++ |
| **Simulation** | Gazebo + URDF |
| **Learning** | Imitation learning — demonstration collection |

## Gallery

<div class="project-gallery">
  {% for item in page.gallery %}
    {% if item.type == "image" %}
      <img src="{{ item.file | relative_url }}" alt="{{ item.description }}" />
    {% endif %}
  {% endfor %}
</div>

## 3D Model

<div class="project-model">
  <model-viewer src="{{ page.models.first.file | relative_url }}" alt="SAPIENS 3D model" camera-controls auto-rotate style="width:100%; height:400px; background: transparent;">
  </model-viewer>
</div>

## Narrative & Progress

Switzerland’s first student-built humanoid is here, and we’re just getting started 🇨🇭🤖🎀

As part of the SAPIENS project at AI Team - Robotics, eight of us built Mina using Berkeley Humanoid Lite as our open-source base. The goal was to deeply understand every subsystem: actuation, electronics, mechanical integration, and the software stack that ties it all together while iterating and customizing where necessary.

From there, we’re pushing further:

→ Custom four-fingered hands, fully designed and built in-house

→ Teleoperation using VR headset and custom gloves with flex sensors and IMUs for demonstration data collection

→ Computer vision for object detection and grasp targeting

→ An imitation learning pipeline to train Mina to autonomously grasp objects

Target: autonomous navigation and grasping within one month 🚀

None of this would be possible without an ambitious, talented, and motivated team. I’m honored to be leading this project alongside Darius Giannoli and teammates Alexandre, Edoardo, Edgard, Karol, Mattia & Tristan.

Now back to debugging (& reprinting broken parts).

---
