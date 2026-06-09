---
layout: project
title: "3U CubeSat Qualification Dispenser"
description: "Redesigned and manufactured a 3U CubeSat qualification dispenser for the CHESS mission; verified first natural frequency 2060.6 Hz via Ansys FEM."
date: 2026-05-01
categories: [Aerospace, Structural Engineering]
tags: [Ansys FEM, SolidWorks, ECSS Standards, NASA GEVS, Vibration Testing, Al 7075-T6, CNC Machining]
featured_image: "/assets/images/projects/cubesat/photo-01.jpg"
period: "Spring Semester 2026"
organisation: "EPFL Spacecraft Team - Structures Pole"
type: "MA Semester Project"
status: "Completed (vibration test campaign pending)"
github_url: ""

# 3D Models - placeholder for later .glb
models:
  - file: "/assets/models/cubesat-dispenser.glb"
    description: "CubeSat dispenser placeholder model (drop .glb at assets/models/cubesat-dispenser.glb)"

# Photo gallery placeholders
gallery:
  - type: "image"
    file: "/assets/images/projects/cubesat/photo-01.jpg"
    description: "Dispenser overview"
  - type: "image"
    file: "/assets/images/projects/cubesat/photo-02.jpg"
    description: "Top plate and rail detail"
  - type: "image"
    file: "/assets/images/projects/cubesat/photo-03.jpg"
    description: "Helicoil inserts and fasteners"
  - type: "image"
    file: "/assets/images/projects/cubesat/photo-04.jpg"
    description: "CNC machined parts"
  - type: "image"
    file: "/assets/images/projects/cubesat/photo-05.jpg"
    description: "Assembly and fit checks"
  - type: "image"
    file: "/assets/images/projects/cubesat/photo-06.jpg"
    description: "Inspection and surface finish"

components:
  - name: "Material"
    quantity: "Many"
    description: "Al 7075-T6"
  - name: "Fasteners"
    quantity: "Multiple"
    description: "M8 with Helicoil inserts; M10 for shaker interface"

---

## Project Overview

The EPFL Spacecraft Team is developing CHESS - two 3U CubeSats for atmospheric research, planned for launch in 2027. Before flight, the satellites must pass a qualification vibration test campaign on a shaker table. The dispenser is a structural fixture that holds the CubeSat and reproduces launch boundary conditions.

A first-generation dispenser failed its test campaign at the University of Bern in late 2025. This semester project re-designed the dispenser, verified it by FEM, manufactured it, and prepared it for a second test campaign.

## What went wrong with the previous dispenser

- Insufficient stiffness - resonant modes fell inside the 0-2000 Hz test band, invalidating the test
- Fastener failures - threads stripped, screws loosened (no secondary locking)
- Wrong tolerances - CubeSat mass model did not slide freely; wear marks from relative movement during testing
- Top plate bending - plate deflected under load and contacted the CubeSat, creating unintended constraints

## My redesign - key decisions

- Closed-box structure replacing the open-frame prototype - substantially stiffer in all three axes and in torsion
- Redundant shaker table interface - 2x M10 bolts per bracket (5 brackets per side) on 80 mm grid, compatible with University of Bern shaker table
- Helicoil inserts for all M8 fasteners - thread engagement of 1.5d = 12 mm (vs ~2 mm originally)
- Loctite 243 secondary locking on all M8 bolts
- Internal top plate rails - reduce unsupported span and prevent out-of-plane bending
- H7/h6 clearance fit on rail guide channels - CubeSat slides freely under its own weight
- Type III hard anodizing (MIL-A-8625) on rail contact surfaces - Ra <= 1.6 µm, prevents cold welding
- Sensor access holes in top plate for accelerometer cables
- Material: Al 7075-T6 throughout - yield strength 503 MPa, compatible with hard anodizing

## FEM Results (Ansys Mechanical 2024 R2)

| Analysis | Requirement | Result | Margin | Status |
|---|---:|---:|---:|:---:|
| Modal - 1st natural frequency | > 2000 Hz | 2060.6 Hz | +3.0% | ✓ Pass |
| Random vibration - peak stress (3σ, NASA GEVS) | < 503 MPa | 56.9 MPa | +7.84 | ✓ Pass |
| Quasi-static - mean structural stress (20g) | MOS >= 0 | 9.09 MPa | +43.2 | ✓ Pass |

First three mode shapes: top plate bending at 2060.6 Hz, pusher plate bending at 2355.8 Hz, side panel bending at 2981.8 Hz.

## Manufacturing

- 17 machined parts, all Al 7075-T6, CNC milled at Satellis workshop
- Critical features: H7/h6 rail guide channels, flatness of mating faces, Helicoil insert depth, M10 bolt pattern on 80 mm grid
- Post-machining inspection: dimensional check, fit check (mass model slides freely), surface roughness certificate
- Assembly: L-brackets -> side panels -> top plate -> CubeSat insertion -> lateral plates -> final torque check

## Status

Design complete, manufactured, assembled. Vibration test campaign at the University of Bern not yet conducted at time of writing - results to be added when available.

## 3D Model

<div class="project-model">
  <model-viewer src="{{ page.models.first.file | relative_url }}" alt="CubeSat dispenser 3D model" camera-controls auto-rotate style="width:100%; height:420px; background: transparent;">
  </model-viewer>
</div>

## Gallery

<div class="project-gallery">
  {% for item in page.gallery %}
    {% if item.type == "image" %}
      <img src="{{ item.file | relative_url }}" alt="{{ item.description }}" />
    {% endif %}
  {% endfor %}
</div>

---
