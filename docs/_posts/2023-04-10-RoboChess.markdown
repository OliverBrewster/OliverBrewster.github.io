---
layout: post
title:  "Robo Chess Project"
date:   2023-04-10 09:32:26 +0000
categories: Engineering Projects
related_image: /assets/RoboChess/Mech2.png
---
<!-- # RoboChess Project -->

### Project Summary:
I proposed and led this project for a full year with the Robotics and Additive Manufacturing Society ([OxRAM](https://www.oxramsociety.org/)). The project aimed to create a fully automated chess board able to move the pieces under the board. The main design constraint of the board was its size, which was required to fit in a small footprint and have a simple interface (no more complicated to use than a pair of wireless headphones!). With 2 hours per week spent on the project, and 30 sessions completed to date, the project has hit the following milestones:
- 64 hall effect sensor array and multiplexing are fully designed and the smaller array is fully tested and working
- Fully 3D printed motion system is working, with motion planner doing inverse kinematics to convert from cartesian (x,y) to (θ1,θ2) scara joint angles.
- Android app is written and interacts with Arduino through Bluetooth module, and LiChess via their API.
- Magnetic engagement and release system tested to reliably move components
- Only *integration hell* remains....

### Contribution to Project:
- Put together a project proposal and recruited a well-equipped team of 8 people to work on it.
- Joined one other in the magnetics/magnetics team to build the motion system and develop a magnetics setup that would work for reliably moving the pieces
- Developed the retraction mechanism using a servo-actuated permanent magnet for engaging and disengaging pieces.
- Made the argument for a scara-type mechanism for traversing X-Y space over a cartesian mechanism using wires. Contributed to CADing (modifying parts for printability, and adding cable management to end effector using slip ring)
- Integrated retraction mechanism as end effector and tuned magnet/retraction height to consistently grip pieces.
- Advertised the project at Oxford's first RepRap festival and got featured by a popular 3D printing YouTuber!

### Gallery
<div style="display: grid; grid-template-columns: 0.5fr 0.589fr;">
  <img src="/assets/RoboChess/TheTeam.jpg" alt="RoboChess Team" style="max-width: 100%;">
  <img src="/assets/RoboChess/YouTube.png" alt="YouTube feature" style="max-width: 100%;">
</div>

<div style="display: grid; grid-template-columns: 1fr;">
  <img src="/assets/RoboChess/EarlyTest.gif" alt="Early board test" style="max-width: 100%;">
</div>

<div style="display: grid; grid-template-columns: 0.5fr 0.5fr;">
  <img src="/assets/RoboChess/Mech2.PNG" alt="Mechanism 1" style="max-width: 100%;">
  <img src="/assets/RoboChess/Mech1.PNG" alt="Mechanism 2" style="max-width: 100%;">
</div>