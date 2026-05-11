---
layout: page
title: DetPO — Few-Shot Object Detection via Prompt Optimization
description: In-Context Learning with Multi-Modal LLMs · ECCV Under Review
img: assets/img/projects/detpo.png
importance: 2
category: Research
---

**Status:** Under Review — ECCV (Rebuttal)

**Links:** [Paper](https://arxiv.org/abs/2603.23455) &nbsp;|&nbsp; [PDF](https://arxiv.org/pdf/2603.23455)

---

## Overview

Multi-Modal LLMs (MLLMs) demonstrate strong visual grounding on benchmarks like OdinW-13 and RefCOCO. However, state-of-the-art models still struggle to generalize to out-of-distribution classes, tasks, and imaging modalities not encountered during pre-training. Naively adding few-shot visual examples to a prompt often *hurts* detection accuracy compared to prompting with class names alone — suggesting that current MLLMs cannot yet effectively exploit rich multimodal context for object detection.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/detpo.png" title="DetPO Overview" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  DetPO iteratively refines text-only prompts using few-shot visual training examples to improve detection accuracy without model fine-tuning.
</div>

## Motivation

Since frontier MLLMs are typically only accessible via APIs and open-weights models are prohibitively expensive to fine-tune on consumer hardware, there is a strong need for black-box, gradient-free approaches to adapt these models for specialized detection tasks.

## Approach

This work proposes **Detection Prompt Optimization (DetPO)**, a gradient-free test-time optimization approach that iteratively refines text-only prompts by maximizing detection accuracy on few-shot visual training examples, while simultaneously calibrating prediction confidence. DetPO requires no access to model internals and works entirely through API calls.

## Results

DetPO yields consistent improvements across generalist MLLMs on **Roboflow20-VL** and **LVIS**, outperforming prior black-box prompt optimization approaches by up to **9.7%**.

## Key Contributions

- Systematic benchmarking revealing that naive in-context prompting consistently hurts MLLM detection accuracy
- A gradient-free, black-box prompt optimization framework for few-shot object detection
- Contrastive prompt refinement using model true positives, false positives, and false negatives
- State-of-the-art results on Roboflow20-VL and LVIS without any model fine-tuning