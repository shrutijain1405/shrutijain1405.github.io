---
layout: page
title: Text-Based Editing of 3D Gaussian Splats
description: Instruction-guided 3D scene editing with Gaussian Splatting
img: assets/img/projects/splatedit.png
importance: 6
category: Projects
---

[Slides](https://docs.google.com/presentation/d/1psjjOVCbpnVsHDlKHE02etKDmhlMOxh1B-Tfz3J53QE/edit)

[Code](https://github.com/Sambhav300899/SplatEdit)

---

{% include figure.html path="assets/img/projects/splatedit.png" title="SplatEdit Pipeline" class="img-fluid rounded z-depth-1" %}

SplatEdit enables text-driven editing of 3D Gaussian Splat scenes by combining the gsplat training pipeline with a Qwen + SAM + Instruct-Pix2Pix editing module that iteratively generates multi-view edited renderings consistent with a natural language instruction (e.g., "make it autumn") and uses them to update the Gaussian Splat parameters, alternating between image editing and Gaussian optimization steps, with CLIP Directional Similarity used as the primary evaluation metric and BLIP-generated captions providing automatic references for the original scenes.