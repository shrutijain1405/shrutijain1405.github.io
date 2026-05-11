---
layout: page
title: Light Weight Character and Shape Recognition for Autonomous Drones
description: ICML 2022 Workshop
img: assets/img/projects/drones.png
importance: 8
category: Research
---

**Venue:** Workshop — ICML 2022

**Links:** [Paper](https://arxiv.org/abs/2208.06804) &nbsp;|&nbsp; [PDF](https://arxiv.org/pdf/2208.06804)

---

## Overview

Unmanned Aerial Vehicles (UAVs) are increasingly deployed in search and rescue missions for tasks such as distributing first aid kits and food packets. For effective operation, these vehicles must reliably identify and distinguish location markers — typically alphanumeric characters superimposed on colored shapes — from aerial imagery. The combinatorial space of shapes, characters, and colors gives rise to a wide variety of such markers, making robust recognition a non-trivial vision problem.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/drones.png" title="Drone Character Recognition Pipeline" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Detection and classification pipeline for alphanumeric characters and shapes in aerial UAV imagery.
</div>

## Approach

This work proposes an object detection and classification pipeline designed to prevent false positives and minimize misclassification of alphanumeric characters and shapes in aerial images. The pipeline combines classical computer vision techniques with unsupervised machine learning for region proposal and target segmentation, followed by a lightweight classification model suitable for deployment directly on aerial vehicles.

Key design choices prioritize **computational efficiency** to ensure real-time performance on the resource-constrained hardware typical of UAV platforms, without sacrificing detection reliability in challenging aerial viewpoints.

This system was developed as part of the team's participation in the **AUVSI-SUAS** (Association for Unmanned Vehicle Systems International — Student Unmanned Aerial Systems) competition.

## Key Contributions

- Lightweight object detection and classification pipeline for aerial marker recognition
- Hybrid approach combining classical CV techniques with unsupervised region proposal
- Deployable on resource-constrained UAV hardware with real-time performance
- Evaluated under AUVSI-SUAS competition conditions