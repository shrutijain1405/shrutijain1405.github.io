---
layout: page
title: "DiffPrompter: Adapting Vision Foundation Models to Adverse Conditions"
description: Learned visual prompts and adapters for robust vehicle segmentation · IROS 2024
img: assets/img/projects/diffprompter.png
importance: 3
category: Projects
---

**Venue:** IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2024)

[Paper](https://arxiv.org/abs/2310.04181)

[Code](https://github.com/DiffPrompter/diff-prompter)

[Project Website](https://diffprompter.github.io/)

[IEEE](https://ieeexplore.ieee.org/document/10802718)

---

{% include figure.html path="assets/img/projects/diffprompter.png" title="DiffPrompter Architecture" class="img-fluid rounded z-depth-1" %}

DiffPrompter adapts vision foundation models using differentiable image preprocessing, learned visual and latent prompts, and adapter modules. I worked on **Parallel (PDA) and Serial (SDA) Differentiable Adaptor** architectures for vehicle foreground segmentation under challenging visual conditions.

Evaluation across driving datasets examines how models trained on **BDD100K** generalize to **ACDC, WildDash, and Dark-Zurich**, while ablations investigate the contributions of preprocessing and latent context.
