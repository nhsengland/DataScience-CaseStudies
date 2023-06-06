---
layout: base
title: Investigating Differential Privacy in a Variational AutoEncoder for Synthetic Data Generation 
permalink: p12_synthvae.html
---

# {{page.title}}
> | "The initial creation of a variational autoencoder with differential privacy for generating single table tabular gaussian data.  This work demonstrated the feasibility of this approach for healthcare and fed into further interactions of the code base."   

<p align="center">
    <img src="assets/img/p12fig1.png" alt=""  width="800"/>
</p>
<p align="left">
    <em>Figure 1: Correlation plots highlighting the difference between the variable relationships in the real and synthetic data across four models.</em>
</p>

This project investigates the potential suitability of Variational Autoencoders (VAEs) as a synthetic data generation tool in the context of the NHS. To effectively address this direction, this work focussed on four key aspects: quality, privacy, ease of use, and interpretability. 

## Results 

We evaluate the performance of the VAE approach alongside five alternative methods available in July/August 2021, namely Gaussian Copula, CTGAN, CopulaGAN, SDV’s TVAE and Independent. Gaussian Copula, CTGAN and CopulaGAN.  Independent refers to our baseline, namely a model which assumes independence across variables.  Evaluating this set of models provides context to the performance of the VAE with respect to both basic (e.g. Independent) and complex (e.g. CTGAN) approaches. 

We found that a variational autoencoder could indeed generate medium to high fidelity synthetic data for a single tabular table with numerical and categorical gaussian variables.   

We then tested how the metrics and visualisations changed when differential privacy was incorporated into the variational autoencoder as a function of differential levels of privacy (increased privacy budget).   As the privacy budget increases, we see the quality decrease as expected.  However, the level of privacy increase associated with increasing the privacy budget appears not to have a direct correlation.  This warrants further work as this might be down to implementation, the metrics being used for evaluation or may point to a feature of the VAE not incorporating the differential privacy correctly. 

| Output | Link | 
| ---- | ---- |
| Open Source Code & Documentation | [Github](https://github.com/nhsx/SynthVAE) |
| Case Study | Awaiting Sign-Off |
| Technical report | [Here](https://github.com/nhsx/SynthVAE/blob/main/reports/report.pdf) |

||||
|:-|:-|:-|
|<img src="assets/img/simulation_badge_S.png" alt  width="80"/>|<img src="assets/img/Synthetic.png" alt  width="80"/>|<img src="assets/img/machine_learning_badge_S.png" alt  width="80"/>|
