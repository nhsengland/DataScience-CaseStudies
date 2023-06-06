---
layout: base
title: Applying our SynPath Simulator to a Diabetes Pathway 
permalink: p11_synpathdiabetes.html
---

# {{page.title}}
> | "Exploration work into incorporating learning into a pathway simulator for diabetes.  This work has fed our current SynPathGo project to create synthetic patient pathways and a foundation for agent based modelling in the NHS."   

<p align="center">
    <img src="assets/img/p11fig1.png" alt=""  width="800"/>
</p>
<p align="left">
    <em>Figure 1: Table of learning algorithms considered for the simulation inteligence layer </em>
</p>

Using the SynPath framework we created a diabetes simulation for 800 patients.  These patients could interact within a fictional local area with hospitals providing outpatient and inpatient services, GP practices and community healthcare services.  

## Results 

The project showed how to develop a set of environments, interactions and patients from academic literature, policy, and clinical resources. The model currently runs a simulation that prints outputs of patient records into the console. It showed that it is possible to gain most of the inputs for a model that model’s outcomes from the academic literature and NHS data. It will be important to make sure that these are up to date and captured for every service in the improvements to the model. When the project is extended it will have the ability to show system effects in healthcare pathways, and the diabetes pathway proof of concept is a crucial step towards this. The implication for clinicians is that they will be able to see the cumulative effects of healthcare interventions (potentially when a novel approach is added). For policymakers, there may be an opportunity to see what the impact of an intervention is pre-implementation on key outcomes when this type of model reaches its full potential.  

| Output | Link | 
| ---- | ---- |
| Open Source Code & Documentation | [Github](https://github.com/nhsx/SynPath\_Diabetes) |
| Case Study | Awaiting Sign-Off |
| Technical report | [Here](https://github.com/nhsx/SynPath\_Diabetes/blob/main/t2dm/reports/Technical%20Report%20(SynPath%20Diabetes)%20v1.pdf) |

||||
|:-|:-|:-|
|<img src="assets/img/simulation_badge_S.png" alt  width="80"/>|<img src="assets/img/Synthetic.png" alt  width="80"/>|<img src="assets/img/machine_learning_badge_S.png" alt  width="80"/>|
