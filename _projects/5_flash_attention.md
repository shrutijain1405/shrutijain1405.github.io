---
layout: page
title: Benchmarking Flash-Attention and Variants for ViT
description: Efficient attention mechanisms for Vision Transformers
img: assets/img/projects/flash_attention.png
importance: 5
category: Course Projects
---

**Links:** [Poster](https://docs.google.com/presentation/d/1fQuShGARc7tGigU-SwInjhqPtVhAYav6_uwPYCFloDI/edit) &nbsp;|&nbsp; [Code](https://github.com/shrutijain1405/Minitorch-flash-attention)

---

## Overview

The quadratic memory and compute complexity of standard self-attention is a fundamental bottleneck for scaling Vision Transformers (ViTs) to high-resolution inputs. Flash-Attention addresses this by reordering the attention computation to be IO-aware — minimizing GPU HBM reads and writes through tiling and online softmax — achieving significant speedups without approximation.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/flash_attention.png" title="Flash Attention Benchmark Results" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Benchmarking memory usage and throughput across standard attention, Flash-Attention, and its variants in a ViT setting.
</div>

## Approach

This project implements and benchmarks Flash-Attention and several of its variants within a custom ViT implementation built on **Minitorch** — a from-scratch deep learning framework implemented in Python and CUDA. The benchmark evaluates:

- **Wall-clock time** and **memory usage** across sequence lengths and batch sizes
- **Numerical correctness** of attention outputs relative to standard attention
- **Scaling behavior** with respect to image resolution and patch size

Multiple Flash-Attention variants are compared, including standard Flash-Attention, block-sparse attention, and multi-query attention, to understand trade-offs across throughput, memory, and accuracy for ViT workloads.

## Key Contributions

- Implementation of Flash-Attention and variants in CUDA within the Minitorch framework
- Comprehensive benchmarking study across sequence length, batch size, and model scale
- Analysis of memory-throughput trade-offs for ViT-specific attention patterns