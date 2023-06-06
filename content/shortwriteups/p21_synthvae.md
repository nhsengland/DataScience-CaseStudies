---
layout: base
title: Developing our SynthVAE code
permalink: p21_synthvae2.html
---

# {{page.title}}
> | "A continuation of the development of our variational autoencoder, this project focused on non-Gaussian input data, hypertuning the code and starting to consider how fairness in the created data can be assessed and implemented.  This project has fed into future development work of turning this code into a production level tool."   

<p align="center">
    <img src="assets/img/p21fig1.png" alt=""  width="800"/>
</p>
<p align="left">
    <em>Figure 1: Directed Acylic Graph (DAG) of a network of variables highlighting their relationships.  The highlighted blue I node is the variable of interest whilst the other highlighted blue node is the sensitive vraiable that maybe inducing bias.</em>
</p>

Continued the previous development of our VAE to correct for an error discovered since the last project finished.  This error appears when trying to generate data for continuous variables which follow non-Gaussian distributions.  Previously, standard scaling had been used to normalise these variables which was causing the non-gaussian variables to be synthesised poorly.  This was replaced with a Guassian mixture model from the RDT python library to scale and transform these variables into ones with a Gaussian distribution. The second phase of this worked focussed on understanding the different ways of measuring and implementing fairness within the synthetic data.   

## Results 

There are many metrics to choose from to measure fairness and to make the situation more complex, not all metrics are compatible with one another, i.e. you can usually only satisfy one metric at a time. This means that the level of fairness required is project specific and has to be re-evaluated depending on the research needs. 

| Output | Link | 
| ---- | ---- |
| Open Source Code & Documentation | [Github](https://github.com/nhsx/SynthVAE) |
| Case Study | Awaiting Sign-Off |
| Technical report | [Here](https://github.com/nhsx/SynthVAE/blob/main/reports/NHSXSynthVAE%20(2).pdf) |

||||
|:-|:-|:-|
|<img src="assets/img/simulation_badge_S.png" alt  width="80"/>|<img src="assets/img/Synthetic.png" alt  width="80"/>|<img src="assets/img/machine_learning_badge_S.png" alt  width="80"/>|
