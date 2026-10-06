---
layout: page
title: "Auto Edit: Language-Guided Subject Tracking and Video Reframing"
description: Visual grounding, trajectory verification, and temporal consistency in a shipped video system · Flowstate AI
img: assets/img/projects/auto_edit.png
importance: 0
category: Projects
---

**Role:** Computer Vision Research Engineer Intern — Flowstate AI

[Slide Deck]({{ '/assets/presentations/auto-edit/' | relative_url }})

---

{% include figure.html path="assets/img/projects/auto_edit.png" title="Auto Edit: Language-Guided Subject Tracking and Video Reframing" class="img-fluid rounded z-depth-1" %}

I built and shipped an end-to-end video-editing system that translates a creative brief into subject selection, tracking, and stable vertical framing. The pipeline combines VLM-based grounding, SAM3 tracking, and trajectory verification, with automated correction of unreliable trajectories.

Introducing automated jerk detection and correction improved soccer-ball tracking precision by **15.4%**. My work also covered scene- and shot-level workflow orchestration in **Temporal** and component-level evaluation of tracking, framing stability, latency, and cost.
