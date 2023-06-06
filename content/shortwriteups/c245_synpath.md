---
layout: base
title: Building the Foundations for a Generic Patient Simulator 
permalink: c245_synpath.html
---


# {{page.title}}

> | "Would an agent-based simulation approach allow synthetic patient pathways and scenario modelling to be created for healthcare specific implementations.  "   



<p align="center">
    <img src="assets/img/c245fig1.png" alt="Overview of data model"  width="800"/>
</p>
<p align="left">
    <em>Figure 1: Overview of the Synpath data model</em>
</p>

A data model (“Patient Agent”) was developed for fake patients to be defined in the simulation.  The patient is then assigned a health record (conditions, medications,  ..) with optional additional attributes. An environment layer, representing the physical and abstract health system the patient can interact with (e.g., GP practice, multidisciplinary team meeting) can then update the patient record with appointment times, updates to health status or increase in medications prescribed.  

## Results 

Foundations were built for the data model and environment.   During the development it became clear that a key nature to be included for healthcare agent simulations in the NHS is the distinction between active and passive agents in regards to the choice of the next environment interaction point.   Efficient object communication and concurrency were also highlighted needed significant further development. 

| Output | Link | 
| ---- | ---- |
| Open Source Code & Documentation | [Github](https://github.com/nhsx/SynPath) |
| Case Study | Awaiting Sign-Off |
| Technical report | [Here](https://github.com/nhsx/SynPath/blob/master/reports/REDACTED_C245%20ABM%20Patient%20Pathways_Final%20Report_V3_28042021.cleaned.pdf) |

||||
|:-|:-|:-|
|<img src="assets/img/simulation_badge_S.png" alt  width="80"/>|<img src="assets/img/Synthetic.png" alt  width="80"/>|<img src="assets/img/machine_learning_badge_S.png" alt  width="80"/>|