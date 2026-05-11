---
layout: page
title: Light Weight Character and Shape Recognition for Autonomous Drones
description: Workshop — ICML 2022
img: assets/img/projects/drones.png
importance: 8
category: Projects
---

**Venue:** Workshop — ICML 2022

[Paper](https://arxiv.org/abs/2208.06804)

[PDF](https://arxiv.org/pdf/2208.06804)

---

{% include figure.html path="assets/img/projects/drones.png" title="Drone Character Recognition Pipeline" class="img-fluid rounded z-depth-1" %}

This work proposes a lightweight object detection and classification pipeline for recognizing alphanumeric characters superimposed on colored shapes in aerial UAV imagery — a task central to the AUVSI-SUAS competition, where drones must reliably identify location markers across a combinatorial space of shapes, characters, and colors. The pipeline combines classical computer vision techniques with unsupervised machine learning for region proposal and target segmentation, followed by a computationally efficient classification model designed to run in real time on the resource-constrained hardware typical of aerial platforms.