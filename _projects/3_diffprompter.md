---
layout: page
title: DiffPrompter — Visual Prompting for Segmentation in Adverse Conditions
description: Differentiable Implicit Visual Prompts · IROS 2024
img: assets/img/projects/diffprompter.png
importance: 3
category: Research
---

**Venue:** IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2024)

**Links:** [Paper](https://arxiv.org/abs/2310.04181) &nbsp;|&nbsp; [Code](https://github.com/DiffPrompter/diff-prompter) &nbsp;|&nbsp; [Project Website](https://diffprompter.github.io/) &nbsp;|&nbsp; [IEEE](https://ieeexplore.ieee.org/document/10802718)

---

## Overview

Semantic segmentation in adverse weather conditions — rain, fog, snow, nighttime — is a critical challenge for autonomous driving systems. While large foundation models have shown great promise across vision tasks, they require specialized adaptation mechanisms when confronted with out-of-distribution, real-world adverse conditions.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/diffprompter.png" title="DiffPrompter Architecture" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  DiffPrompter uses differentiable visual and latent prompts to adapt foundation models for semantic segmentation under adverse weather conditions.
</div>

## Approach

This work introduces **DiffPrompter**, a novel differentiable visual and latent prompting mechanism designed to expand the learning capabilities of existing adaptors in foundation models. The key components include:

- **∇HFC Block:** A differentiable High Frequency Components image processing block that excels at extracting structure in adverse weather where conventional preprocessing fails.
- **DiffVP:** A Differentiable Visual Prompt block that jointly learns visual prompts using DiffIP and latent prompts via a shallow vision encoder.
- **Parallel and Serial Architectures:** Two adaptor variants — Parallel Differentiable Adaptor (PDA) and Serial Differentiable Adaptor (SDA) — are proposed, each suited to different segmentation scenarios.

## Results

DiffPrompter achieves state-of-the-art performance on multiple adverse-condition segmentation benchmarks including **BDD100K**, **ACDC**, **WildDash**, and **Dark-Zurich**, outperforming prior methods EVP and SAM-Adapter.

## Key Contributions

- Differentiable visual and latent prompting mechanism for foundation model adaptation
- ∇HFC image processing block tailored for adverse weather feature extraction
- Jointly training visual and latent prompts yields strong out-of-distribution generalization
- Two adaptor architectures (PDA, SDA) achieving state-of-the-art results