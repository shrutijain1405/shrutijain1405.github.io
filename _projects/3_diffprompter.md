---
layout: page
title: DiffPrompter — Visual Prompting for Segmentation in Adverse Conditions
description: Differentiable Implicit Visual Prompts · IROS 2024
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

DiffPrompter introduces a novel differentiable visual and latent prompting mechanism for adapting foundation models to semantic segmentation under adverse weather conditions such as rain, fog, snow, and nighttime driving. The approach proposes a ∇HFC image processing block that excels at extracting structure in challenging conditions where conventional preprocessing fails, and jointly trains visual and latent prompts through Parallel (PDA) and Serial (SDA) Differentiable Adaptor architectures — achieving state-of-the-art out-of-distribution segmentation performance on BDD100K, ACDC, WildDash, and Dark-Zurich, outperforming prior methods EVP and SAM-Adapter.