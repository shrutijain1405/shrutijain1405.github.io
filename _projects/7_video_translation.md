---
layout: page
title: Video Translation with Voice Cloning and Lip Sync
description: End-to-end pipeline for cross-lingual video dubbing
img: assets/img/projects/video_translation.png
importance: 7
category: Course Projects
---

**Links:** [Code](https://github.com/shrutijain1405/VideoTranslation)

---

## Overview

Dubbed video content that faithfully preserves the speaker's voice and maintains lip synchronization is a challenging multimodal problem requiring the integration of speech recognition, machine translation, voice cloning, audio-visual alignment, and lip synthesis. This project develops an end-to-end pipeline for cross-lingual video translation from English to German, with temporal audio synchronization and neural lip syncing.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/video_translation.png" title="Video Translation Pipeline" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  End-to-end video translation pipeline: transcript parsing → text translation → voice cloning → audio synchronization → lip sync.
</div>

## Pipeline

The system proceeds through the following stages:

1. **Transcript Parsing:** SRT subtitle files are parsed to extract transcript segments and their precise timestamps.
2. **Text Translation with Length Matching:** Segments are translated from English to German using the `opus-mt-en-de` model. A `flan-t5-small` model then rewrites translations to match the character length of the source, preserving semantic content while enabling temporal alignment.
3. **Audio Segmentation:** The input audio is extracted from the video using `ffmpeg` and split into per-segment clips aligned with the transcript timestamps.
4. **Voice Cloning TTS:** Per-segment German translations are synthesized using `coqui-tts` with the `tacotron2-DDC` German model, preserving speaker-like characteristics.
5. **Audio Time Synchronization:** Each translated audio segment is time-stretched or compressed using `librosa` to match the duration of the corresponding source segment, with silence padding for residual gaps.
6. **Merging and Global Sync:** All synchronized segments are merged and globally aligned with the source audio to ensure final duration parity.
7. **Lip Synchronization:** The translated audio is synchronized with the original speaker's lip movements using **LatentSync**, producing a visually coherent dubbed video.

## Key Contributions

- Full end-to-end pipeline from raw video to dubbed, lip-synced output
- Length-constrained translation using LLM rewriting to enable temporal alignment
- Voice cloning TTS with per-segment audio time synchronization using librosa
- Integration of LatentSync for neural lip synchronization