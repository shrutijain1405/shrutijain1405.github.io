---
layout: page
title: Text-Based Editing of 3D Gaussian Splats
description: Instruction-guided 3D scene editing with Gaussian Splatting
img: assets/img/projects/splatedit.png
importance: 6
category: Course Projects
---

**Links:** [Slides](https://docs.google.com/presentation/d/1psjjOVCbpnVsHDlKHE02etKDmhlMOxh1B-Tfz3J53QE/edit) &nbsp;|&nbsp; [Code](https://github.com/Sambhav300899/SplatEdit)

---

## Overview

3D Gaussian Splatting (3DGS) has emerged as a powerful representation for novel view synthesis, offering real-time rendering with high visual fidelity. A key open challenge is enabling intuitive, instruction-guided editing of these representations — allowing users to modify 3D scenes using natural language without requiring expert knowledge of the underlying 3D structure.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/splatedit.png" title="SplatEdit Pipeline" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Text-driven editing of 3D Gaussian Splat scenes using a multi-view Instruct-Pix2Pix pipeline with iterative Gaussian updates.
</div>

## Approach

SplatEdit builds on the **gsplat** pipeline for training base Gaussian Splats and extends it with a text-conditioned editing module. The editing pipeline proceeds as follows:

1. A base 3D Gaussian Splat is trained on a target scene using multi-view RGB images.
2. A **Qwen + SAM + Instruct-Pix2Pix** pipeline generates edited 2D renderings consistent with the provided text instruction (e.g., *"make it autumn"*).
3. Edited multi-view images are used to iteratively update the Gaussian Splat parameters, alternating between image editing and Gaussian optimization steps.
4. Evaluation is performed using **CLIP Directional Similarity** between original and edited scene captions, with BLIP used to generate automatic captions for the original scenes.

## Key Contributions

- End-to-end pipeline for text-driven 3D Gaussian Splat editing
- Iterative multi-view editing strategy using Instruct-Pix2Pix for consistent 3D updates
- CLIP-based evaluation framework for measuring semantic fidelity of scene edits
- Experiments across diverse indoor and outdoor scenes from the 360° dataset