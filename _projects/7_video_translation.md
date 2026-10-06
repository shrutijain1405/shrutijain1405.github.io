---
layout: page
title: Multimodal Video Dubbing with Temporal Alignment
description: Coordinating language, speech generation, audio timing, and lip synchronization
img: assets/img/projects/video_translation.png
importance: 7
category: Projects
---

[Code](https://github.com/shrutijain1405/VideoTranslation)

---

{% include figure.html path="assets/img/projects/video_translation.png" title="Video Translation Pipeline" class="img-fluid rounded z-depth-1" %}

I built an English-to-German video-dubbing pipeline that integrates translation, voice-cloned speech synthesis, audio-duration alignment, and lip synchronization. The system coordinates text, audio, and visual outputs at the segment level to fit translated speech to the original video.

The implementation parses **SRT transcripts**, uses **opus-mt-en-de and flan-t5-small** for length-constrained translation, and combines **Coqui TTS**, **librosa** audio synchronization, and **LatentSync** lip synchronization. The project demonstrates integration of multiple pretrained models and explicit handling of temporal alignment across modalities.
