---
layout: base
title: Investigating Applying and Evaulating a Language Model to Patient Safety Data 
permalink: p33_patientsafetylms.html
---

# {{page.title}}
> | "What's the most suitable models and workflows for represneting an NHS text dataset?"   

<p align="center">
    <img src="assets/img/p33fig1.png" alt=""  width="100%"/>
</p>
<p align="center">
    <em>Figure 1: Taken from DeCLUTR: Deep Contrastive Learning for Unsupervised Textual Representations - arXiv:2006.03659</em>
</p>

In collaboration with the NHS England patient safety data team, we present an exploration of a selection of different language model pretraining and finetuning objectives with patient safety incident reports as the domain of interest, followed by a discussion of a number of methods for probing and evaluating these new models, and their respective embedding spaces.

## Results 

Results showed that the models trained on the patient safety incident reports using either the Masked Language Model (MLM) objective, or the MLM plus contrastive loss objective, appeared to have a superior performance on the presented pseudo-tasks when compared to their general domain equivalent. Whilst the performance in the frozen setting did not match that of the full fine-tuned setting, we have not performed a thorough investigation, for instance we could look to utilising larger base models. Further there are other examples of promising approaches which can better utilise frozen language models at scale, such as prompt learning and parameter efficient fine-tuning.


| Output | Link | 
| ---- | ---- |
| Open Source Code & Documentation | [Github](https://github.com/nhsx/ELM4PSIR) |
| Case Study | Awaiting Sign-Off |
| Technical report | [Here](https://github.com/nhsx/ELM4PSIR/blob/main/reports/ELM4PSIR_NT_v1.1.pdf) |

|:-|:-|:-|
|<img src="assets/img/machine_learning_badge_S.png" alt  width="80"/>|
