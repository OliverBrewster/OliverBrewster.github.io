---
layout: post
title:  "Experimental Birdflight"
date:   2022-05-15 09:32:26 +0000
categories: Engineering Projects
---
<!-- # RoboChess Project -->

### Project Summary:
This project was undertaken for a friend writing a master's in biology, to understand how the stability of bird flight changes as the center of mass is shifted along the body of the bird. Experimental data was used to get the surface of the bird in many flight positions and the requirement was to build an experiment to shift COM along the center chord of the bird.

The result of this work was extremely well received and is being published in an academic paper (for which I will be a contributor). Among the master's cohort in Biology, it placed second in the year and won the prize in computational biology.

### Main Challenges
A significant challenge of this project was constraints in manufacturing. These models were to be printed on a cheap SLA printer (Creality). This meant splitting the models and joining them with dowels. 

Producing the experimental setup from bird data posed a challenge too. The system to shift COM had to be as discrete as possible, while also shifting enough mass to move between the stable flight mode and unstable flight mode.

<div style="display: grid; grid-template-columns: 0.5fr 0.5fr;">
  <img src="/assets/Birdflight/Bird_Flight.jpeg" alt="Birdflight 1" style="max-width: 100%;">
  <img src="/assets/Birdflight/Completed_Hardware.jpeg" alt="Birdflight 2" style="max-width: 100%;">
</div>

### Contribution
The resources on the input for this project were surfaces produced from point cloud data of birds and an incomplete idea of wanting to design an experiment that could test for stability and instability in bird flight.

The timeline was extremely strict, with only a few weeks to go from idea to experimental results. I pushed the manufacturing towards SLA, which I knew could produce the intricate details of the model, with a good surface finish. I then developed the method of shifting a mass along a metal rod and produced the design to make this feasible on the model. After an initial prototype and successful testing, this design was ported to four other birds, producing a fleet that would go on to produce successful experimental results (which was firmly out of my hands!)

<div style="display: grid; grid-template-columns: 1fr 1fr;">
  <img src="/assets/Birdflight/Experimental.jpeg" alt="Birdflight 3" style="max-width: 100%;">
  <img src="/assets/Birdflight/Five_Birds.jpeg" alt="Birdflight 4" style="max-width: 100%;">
</div>