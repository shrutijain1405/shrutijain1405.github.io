---
layout: page
title: Multimodal Medical Triaging on UAV Data
description: DARPA Triage Challenge — AIRLab, CMU
img: assets/img/projects/darpa_triage.png
importance: 1
category: Research
---

**Advisors:** Prof. John Galeotti and Prof. Sebastian Scherer, AIRLab, Carnegie Mellon University

**Links:** [Project Website](https://mscvprojects.ri.cmu.edu/2026teamf21/) &nbsp;|&nbsp; [Poster](https://drive.google.com/file/d/1B4ta0mYtSjabW7_4Pv8o20r-UGhR_sjz/view)

---

## Overview

The DARPA Triage Challenge aims to enable autonomous systems to rapidly detect and prioritize casualties in disaster scenarios using UAV imagery. This project develops a multimodal medical triaging pipeline that leverages RGB and thermal (IR) drone data to predict 50+ hierarchical medical labels, including hemorrhage, trauma, posture, and respiratory distress.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/darpa_triage.png" title="DARPA Triage Pipeline" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Multimodal triaging pipeline using RGB and thermal UAV imagery for casualty detection.
</div>

## Motivation

A major challenge in this setting is the limited availability of paired RGB–IR training data for medical triage in the wild. Standard supervised approaches fail to generalize to the diverse, cluttered environments encountered in real disaster response scenarios.

## Approach

To address the data scarcity problem, a conditional diffusion model is first trained to synthesize thermal (IR) images from RGB inputs, enabling large-scale synthetic RGB–IR pair generation. These multimodal pairs are then used to fine-tune Vision-Language Models (VLMs) for robust casualty understanding and triage reasoning in complex real-world environments.

The pipeline predicts a rich set of hierarchical medical labels across both imaging modalities, enabling a comprehensive assessment of casualty status directly from drone footage without requiring human intervention.

## Key Contributions

- End-to-end multimodal triaging pipeline operating on live UAV RGB and thermal imagery
- Conditional diffusion-based RGB-to-IR synthesis to overcome paired data scarcity
- Fine-tuning of Vision-Language Models for hierarchical medical label prediction
- System evaluated under DARPA Triage Challenge conditions