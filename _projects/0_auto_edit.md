---
layout: page
title: "Auto Edit: Intelligent Video Reframing Tool"
description: Multimodal computer vision and editorial reasoning · Flowstate AI
img: assets/img/projects/auto_edit.png
importance: 0
category: Projects
---

**Role:** Computer Vision Research Engineer Intern — Flowstate AI

---

{% include figure.html path="assets/img/projects/auto_edit.png" title="Auto Edit: Intelligent Video Reframing Tool" class="img-fluid rounded z-depth-1" %}

Auto Edit is a multimodal computer vision system that turns long-form horizontal video into story-aware vertical edits. Instead of treating the task as a simple center crop, the system first reasons about which moments satisfy a creative brief, then decides how each selected shot should be framed for a 9:16 canvas.

I worked across the system end to end: translating creative intent and video context into editable story plans, building shot-aware subject grounding and tracking, composing stable vertical framing, and creating evaluation signals for motion, composition, and narrative quality. Human review remains part of the workflow through transparent scene and framing decisions that can be retimed, reordered, or refined.

The interactive presentation includes playable examples of the resulting edits and is designed to open directly in the browser.

[Open the Auto Edit presentation]({{ '/assets/presentations/auto-edit/' | relative_url }})
