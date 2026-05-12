---
layout: page
title: DetPO — Few-Shot Object Detection via Prompt Optimization
description: In-Context Learning with Multi-Modal LLMs · ECCV Under Review
img: assets/img/projects/detpo.png
importance: 2
category: Projects
---

**Status:** Under Review — ECCV (Rebuttal)

[Paper](https://arxiv.org/abs/2603.23455)
[Website](https://ggare-cmu.github.io/DetPO/)
[Code](https://github.com/ggare-cmu/DetPO)

<!-- [PDF](https://arxiv.org/pdf/2603.23455) -->

---

{% include figure.html path="assets/img/projects/detpo.png" title="DetPO Overview" class="img-fluid rounded z-depth-1" %}

Multi-Modal LLMs exhibit strong visual grounding on standard benchmarks but struggle to generalize to out-of-distribution classes, tasks, and imaging modalities — and naively adding few-shot visual examples to a prompt often hurts detection accuracy compared to prompting with class names alone. This work proposes Detection Prompt Optimization (DetPO), a gradient-free, black-box test-time optimization approach that iteratively refines text-only prompts by maximizing detection accuracy on few-shot visual training examples while calibrating prediction confidence, achieving consistent improvements across generalist MLLMs on Roboflow20-VL and LVIS and outperforming prior black-box approaches by up to 9.7% without any model fine-tuning.