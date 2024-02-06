---
layout: post
title:  "Robo Chess Project"
date:   2023-04-10 09:32:26 +0000
categories: Engineering Projects
related_image: /assets/RoboChess/Mech2.png
---
<!-- # RoboChess Project -->

### Project Summary:
I proposed and lead this project for a full year with the robotics and additive manufacturing society ([OxRAM](https://www.oxramsociety.org/)). The aim of the project was to create a fully automated chess board able to move the pieces under the board. The main design constraint of the board was its size, which was required to fit in a small footprint and have a simple interface (no more complicated to use than a pair of wireless headphones!). With 2 hours per week spent on the project, and 30 sessions completed to-date, the project has hit the following milestones:
- 64 hall effect sensor array and multiplexing is fully designed and smaller array fully tested and working
- Fully 3D printed motion system is working, with motion planner doing inverse kinematics to convert from cartesian (x,y) to (θ1,θ2) scara joint angles.
- Android app written and interacting with arduino through bluetooth module, and LiChess via their API.
- Magnetic engagement and release system tested to reliably move components
- Only *integration hell* remains....

### Contribution to Project:
- Put together project proposal and recruited well-equipped team of 8 people to work on it.
- Joined one other in the magnetics/magnetics team to build the motion system and develop a magnetics setup that would work for reliably moving the pieces
- Developed the retraction mechanism using a servo actuated permenant magnet for engaging and disengaging pieces.
- Made the argument for scara-type mechanism for traversing X-Y space over cartesian mechanism using wires. Contributed to CADing (modifying parts for printability, and adding cable management to end effector using slip ring)
- Integrated retraction mechanism as end effector and tuned magnet/retraction height to consistently grip pieces.
- Advertised the project at the Oxford's first RepRap festival and got featured by a popular 3D printing YouTuber!

### Gallery
<!-- ![Early Test](/assets/RoboChess/EarlyTest.gif) ![Mechanism 1](/assets/RoboChess/Mech1.PNG)
![Mechanism 2](/assets/RoboChess/Mech2.PNG) ![YouTube feature](/assets/RoboChess/YouTube.png)
![The team](/assets/RoboChess/TheTeam.jpg) -->


<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/RoboChess/TheTeam.jpg" alt="RoboChess Team" style="flex: 1; max-width: 50%;" />
    <img src="/assets/RoboChess/YouTube.png" alt="YouTube feature" style="flex: 1; max-width: 50%;" />
</div>

![Single Image](/assets/RoboChess/EarlyTest.gif)

<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/RoboChess/Mech2.png" alt="RoboChess Team" style="flex: 1; max-width: 50%;" />
    <img src="/assets/RoboChess/Mech1.png" alt="YouTube feature" style="flex: 1; max-width: 50%;" />
</div>