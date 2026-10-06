---
layout: page
title: "DetPO: Prompt Optimization for Few-Shot Object Detection"
description: Adapting multimodal LLMs for detection without weight updates · ECCV 2026
img: assets/img/projects/detpo.png
importance: 2
category: Projects
---

**Status:** Accepted — ECCV 2026

[Paper](https://arxiv.org/abs/2603.23455)

[Website](https://ggare-cmu.github.io/DetPO/)

[Code](https://github.com/ggare-cmu/DetPO)

<!-- [PDF](https://arxiv.org/pdf/2603.23455) -->

---

{% include figure.html path="assets/img/projects/detpo.png" title="DetPO Overview" class="img-fluid rounded z-depth-1" %}

DetPO investigates how to adapt multimodal LLMs to unfamiliar object categories and visual domains with few labeled examples. We found that adding visual demonstrations can reduce detection accuracy, motivating a gradient-free approach that optimizes textual prompts against detection performance while calibrating confidence.

The method improves performance without model fine-tuning, outperforming prior black-box approaches by up to **9.7 mAP** in evaluations involving **Roboflow20-VL and LVIS**.
