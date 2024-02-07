---
layout: post
title:  "Design of Domestic Robot"
date:   2023-02-14 09:32:26 +0000
categories: Engineering Projects
---

### Project Summary:
This was a theory-based design project to develop an autonomous robot for a domestic setting. Our team of four members opted for an elderly care robot and developed all aspects of the design including engineering, aesthetic, and business case. The CAD mock-up I produced for the robot is below:

### Contribution
The different sub-systems of the robot were distributed between members, with me tackling the following four tasks:

#### Aesthetic Design
This involved a CAD mock-up of the robot which was non-imposing while also enabling the complete functionality we had set for the robot. The final design is below:

<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/3YP/BILLY.png" alt="Domestic Care Robot, BILLY" style="flex: 1; max-width: 65%;" />
</div>


#### Object Detection
A feature proposed for this project was the ability of the robot to recognise and retrieve items for a user. I took on the job of object detection (which was proven with the simpler task of collecting mugs). An unlabelled dataset was available for this object class, so algorithm training required the following steps:
- Select a suitable algorithm (YOLOv5 in this case)
- Label a dataset of 1000 images using a Python tool
- Sanitise images for training by fixing the aspect ratio, and binning to a lower resolution
- Apply YOLO algorithm to obtain weights and biases (training results below):
<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/3YP/Training.png" alt="Domestic Care Robot, BILLY" style="flex: 1; max-width: 85%;" />
</div>
- Adjust hyper-parameters (batch size and epoch number) to improve the mean average precision
- Test trained algorithm on several inference tasks, including video feed (static test below)
<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/3YP/Inference.png" alt="Domestic Care Robot, BILLY" style="flex: 1; max-width: 85%;" />
</div>


#### Path Planning
This was an important part of the autonomy of our robot and involved a literature review of computationally efficient methods to produce optimal paths through a known space. Critical to this is configuration space, which reduces the problem to a single point moving through a 3D space. This concept involves 'padding' each object in the map with additional space to account for places the robot can't access due to its size:
<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/3YP/C-Space.png" alt="Domestic Care Robot, BILLY" style="flex: 1; max-width: 65%;" />
</div>

This C-Space is then sampled randomly to produce a graph of the space from which a simple path-finding algorithm such as A* can be implemented from the start node to the end node.