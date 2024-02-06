---
layout: post
title:  "Print Farm Project"
date:   2022-02-14 09:32:26 +0000
categories: Engineering Projects
---
<!-- # RoboChess Project -->

### Project Summary:
This project is the development log of my 3D printing farm which was used to build a small e-commerce business in 2020/2021. The main engineering challenge in this was the optimisation of all parts of the production to get maximum throughput on the machines. This was done through 3 primary methods:
- Optimising individual product GCODEs to decrease print time and increase reliability of prints
- Configuring OctoPrint servers to manage distribution of up-to-date GCODES across all machines. Added benefit of being able to manage all the printers remotely.
- Automated shipping label printing, and system for inventory management to ensure minimal stock was kept of each product.

<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/PrintFarm/FarmV1.gif" alt="Farm V1" style="flex: 1; max-width: 50%;" />
    <img src="/assets/PrintFarm/FarmV2.gif" alt="Farm V2" style="flex: 1; max-width: 50%;" />
</div>

### How it happened:
In 2020, I purchased my first 3D printer (a knackered Anet A8) for £65. Within a few weeks of probing in the dark to debug the machine saw, it pit produced its first successful prints. I used it for a few months, and learnt some basic CAD to start producing my own designs. 

After a little while I saw the potential for prints to be commercialised, and started printing and selling my original designs on eBay (and eventually Etsy). Need for machine capacity led me to get another Anet A8 forming the initial (and small!) print farm just as COVID gripped and free-time became in abundance.

<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/PrintFarm/EarlyFarm.jpg" alt="RoboChess Team" style="flex: 1; max-width: 35%;" />
    <img src="/assets/PrintFarm/FirstPrint.jpg" alt="RoboChess Team" style="flex: 1; max-width: 65%;" />
</div>

Many months of iterating continued as I tested various FDM machines and benchmarked their performance and reliability, debugging a host of issues. Production in the farm was streamlined as I isntalled OctoPrint servers on each printer to allow easy distribution of GCODEs to the growing selection of printers. Production GCODEs were optimised to systematically decrement print times within the limit of each printer.

After settling on a single printer model to focus on, the size of the farm grew with growing sales of printed items. The final result of 1.5yrs of development was 6 optimised printers capable of fulfilling hundreds of order per week. This was a glimpse into satisfaction and pitfulls of manufacturing at medium-scale, which I hadn't seen prior.