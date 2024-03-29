---
layout: post
title:  "3D Print Farm (FDM)"
date:   2022-02-14 09:32:26 +0000
categories: Engineering Projects
---
<!-- # RoboChess Project -->

### Project Summary:
This project is the development log of my 3D printing farm which was used to build a small e-commerce business in 2020/2021. The main engineering challenge in this was the optimisation of all parts of the production to get maximum throughput on the machines. This was done through 3 primary methods:
- Optimising individual product GCODEs to decrease print time and increase the reliability of prints
- Configuring OctoPrint servers to manage the distribution of up-to-date GCODES across all machines. Added benefit of being able to manage all the printers remotely.
- Automated shipping label printing, and system for inventory management to ensure minimal stock was kept of each product.

<div style="display: grid; grid-template-columns: 1fr 1fr;">
  <img src="/assets/PrintFarm/FarmV1.gif" alt="Farm V1" style="max-width: 100%;">
  <img src="/assets/PrintFarm/FarmV2.gif" alt="Farm V2" style="max-width: 100%;">
</div>

### How it happened:
In 2020, I purchased my first 3D printer (a knackered Anet A8) for £65. Within a few weeks of probing in the dark to debug the machine saw, it pit produced its first successful prints. I used it for a few months and learned some basic CAD to start producing my own designs. 

After a little while I saw the potential for prints to be commercialised, and started printing and selling my original designs on eBay (and eventually Etsy). The need for machine capacity led me to get another Anet A8 forming the initial (and small!) print farm just as COVID gripped and free time became in abundance.

<div style="display: grid; grid-template-columns: 0.3656fr 0.65fr;">
  <img src="/assets/PrintFarm/EarlyFarm.jpg" alt="Start of the print farm" style="max-width: 100%;">
  <img src="/assets/PrintFarm/FirstPrint.jpg" alt="Print farm final form" style="max-width: 100%;">
</div>

Many months of iterating continued as I tested various FDM machines and benchmarked their performance and reliability, debugging a host of issues. Production on the farm was streamlined as I installed OctoPrint servers on each printer to allow easy distribution of GCODEs to the growing selection of printers. Production GCODEs were optimised to systematically decrement print times within the limit of each printer.

After settling on a single printer model to focus on, the size of the farm grew with growing sales of printed items. The final result of 1.5 years of development was 6 optimised printers capable of fulfilling hundreds of orders per week. This was a glimpse into the satisfaction and pitfalls of manufacturing at a medium-scale, which I hadn't seen prior.