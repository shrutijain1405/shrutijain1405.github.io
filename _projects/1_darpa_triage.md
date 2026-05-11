---
layout: page
title: Multimodal Medical Triaging on UAV Data
description: DARPA Triage Challenge — AIRLab, CMU
img: assets/img/projects/darpa_triage.png
importance: 1
category: Projects
---

**Advisors:** Prof. John Galeotti and Prof. Sebastian Scherer, AIRLab, Carnegie Mellon University

[Project Website](https://mscvprojects.ri.cmu.edu/2026teamf21/)

[Poster](https://drive.google.com/file/d/1B4ta0mYtSjabW7_4Pv8o20r-UGhR_sjz/view)

---

{% include figure.html path="assets/img/projects/darpa_triage.png" title="DARPA Triage Pipeline" class="img-fluid rounded z-depth-1" %}

This project develops a multimodal medical triaging pipeline for the DARPA Triage Challenge, which aims to enable autonomous systems to rapidly detect and prioritize casualties in disaster scenarios using UAV imagery. The system leverages both RGB and thermal (IR) drone data to predict 50+ hierarchical medical labels — including hemorrhage, trauma, posture, and respiratory distress — addressing the critical challenge of limited paired RGB–IR training data by first training a conditional diffusion model to synthesize thermal images from RGB inputs and then using these synthetic multimodal pairs to fine-tune Vision-Language Models for robust casualty understanding and triage reasoning in complex real-world environments.