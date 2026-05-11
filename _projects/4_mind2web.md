---
layout: page
title: Late-Fusion Gating of Web Agents for MultimodalMind2Web
description: Multimodal web agent grounding with late-fusion gating
img: assets/img/projects/mind2web.png
importance: 4
category: Projects
---

[Poster](https://docs.google.com/presentation/d/1tNBKZ3ycRHwrzGo3Nk0MWN3QJ5GsrUiYiR3hg8GGcoo/edit)

---

{% include figure.html path="assets/img/projects/mind2web.png" title="Late-Fusion Gating Architecture" class="img-fluid rounded z-depth-1" %}

Web agents that autonomously navigate and interact with web interfaces must accurately ground natural language instructions to the correct UI elements, a problem that is significantly harder when both visual and textual context must be jointly understood. This project investigates a late-fusion gating strategy for combining visual and textual modalities in web agent element grounding on the MultimodalMind2Web benchmark, applying gating at the prediction stage so the model can selectively rely on the more informative modality depending on the page context — with systematic ablations across early, late, and gated fusion strategies evaluated over diverse web tasks including search, form filling, and multi-step navigation.