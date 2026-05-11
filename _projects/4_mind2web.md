---
layout: page
title: Late-Fusion Gating of Web Agents for MultimodalMind2Web
description: Multimodal web agent grounding with late-fusion gating
img: assets/img/projects/mind2web.png
importance: 4
category: Course Projects
---

**Links:** [Poster](https://docs.google.com/presentation/d/1tNBKZ3ycRHwrzGo3Nk0MWN3QJ5GsrUiYiR3hg8GGcoo/edit)

---

## Overview

Web agents that autonomously navigate and interact with web interfaces must accurately ground natural language instructions to the correct UI elements. The MultimodalMind2Web benchmark evaluates such agents on real-world web tasks requiring understanding of both textual and visual context — a significantly harder problem than text-only web navigation.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/mind2web.png" title="Late-Fusion Gating Architecture" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Late-fusion gating mechanism combining visual and textual signals for improved web element grounding.
</div>

## Approach

This project investigates a **late-fusion gating** strategy for combining visual and textual modalities in web agent element grounding. Rather than fusing modalities at the input or intermediate representations, gating is applied at the prediction stage — enabling the model to selectively rely on the more informative modality depending on the context of the web page and instruction.

The approach is evaluated on the MultimodalMind2Web benchmark across diverse web tasks including search, form filling, and multi-step navigation.

## Key Contributions

- Late-fusion gating architecture for multimodal web agent element grounding
- Systematic ablation of fusion strategies (early, late, gated) on MultimodalMind2Web
- Analysis of modality contribution across different web task types