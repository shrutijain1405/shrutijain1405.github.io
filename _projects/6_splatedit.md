---
layout: page
title: "SplatEdit: Language-Guided Editing of 3D Scenes"
description: Visual grounding and consistency across views in Gaussian Splat editing
img: assets/img/projects/splatedit.png
importance: 6
category: Projects
---

[Slides](https://docs.google.com/presentation/d/1psjjOVCbpnVsHDlKHE02etKDmhlMOxh1B-Tfz3J53QE/edit)

[Code](https://github.com/Sambhav300899/SplatEdit)

---

{% include figure.html path="assets/img/projects/splatedit.png" title="SplatEdit Pipeline" class="img-fluid rounded z-depth-1" %}

SplatEdit connects natural-language instructions with global and localized edits to 3D Gaussian Splat scenes. The pipeline combines **Qwen/SAM language-guided segmentation**, diffusion-based image editing, and Gaussian optimization, alternating between edited renderings and updates to the 3D representation.

My work included **DDIM inversion and InstructPix2Pix with cross-view attention** to support consistency across viewpoints. The project uses **CLIP Directional Similarity** to evaluate semantic editing direction; this measures instruction alignment rather than multiview consistency itself.
