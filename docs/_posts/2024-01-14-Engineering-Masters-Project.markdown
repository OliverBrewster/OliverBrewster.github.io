---
layout: post
title:  "Hybrid Additive and Subtractive FDM Project"
date:   2024-01-14 09:32:26 +0000
categories: Engineering Projects
---
<!-- # RoboChess Project -->

### Project Summary:
This project aims to develop a Desktop FDM hybrid machine to do both additive and subtractive manufacturing. This has been realised in the form of a modified IDEX machine with one additive tool (Hemera extruder) and one subtractive tool (CNC spindle). With only 3 axes, this system would be very limited in geometry which could be CNC milled. This is why 5-axes have been implemented by adding 2 additional rotation axes to the bed (one with an axis parallel to the y-axis and the other parallel to the z-axis), pictured below:

<div style="display: grid; grid-template-columns: 0.44fr 0.56fr;">
  <img src="/assets/Masters/MachineCAD1.png" alt="CAD 1" style="max-width: 100%;">
  <img src="/assets/Masters/MachineCAD2.png" alt="CAD 2" style="max-width: 100%;">
</div>

### Current Project State
At present, the machine has been fully built and calibrated. All 5 axes are functional, and moves are controlled using GCODE via standard open-source printer hardware. The milling and additive head are independently controllable and can be swapped in and out of use. A stiffer gantry has been fitted to the machine, and the process has started for calibrating optimal CNC parameters. The machine has a ‘digital twin’ which can be used for generating 5-axis milling toolpaths and collision detection.

<div style="display: grid; grid-template-columns: 0.5fr 0.5fr;">
  <img src="/assets/Masters/Benchy.jpg" alt="Benchy Test" style="max-width: 100%;">
  <img src="/assets/Masters/Machine.jpg" alt="POrinter" style="max-width: 100%;">
</div>

### Outstanding Goals
The future goals for the project are the following:
- Use Fusion to generate 3+2-axis milling toolpaths, and write post-processing script to combine with additive GCODE
- Determine optimal cutting parameters for a range of common FDM materials
- Automate the pipeline as much as possible!