---
layout: page
title: Video Translation with Voice Cloning and Lip Sync
description: End-to-end pipeline for cross-lingual video dubbing
img: assets/img/projects/video_translation.png
importance: 7
category: Projects
---

[Code](https://github.com/shrutijain1405/VideoTranslation)

---

{% include figure.html path="assets/img/projects/video_translation.png" title="Video Translation Pipeline" class="img-fluid rounded z-depth-1" %}

This project builds an end-to-end pipeline for cross-lingual video dubbing from English to German, combining transcript parsing from SRT files, length-constrained text translation using opus-mt-en-de and flan-t5-small, per-segment voice cloning TTS with Coqui's Tacotron2-DDC, librosa-based audio time synchronization to match source segment durations, and final lip synchronization using LatentSync — producing a fully dubbed video where the translated speech is temporally aligned with the original speaker's lip movements.