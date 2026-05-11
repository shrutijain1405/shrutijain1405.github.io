---
layout: page
title: Benchmarking Flash-Attention and Variants for ViT
description: Efficient attention mechanisms for Vision Transformers
img: assets/img/projects/flash_attention.png
importance: 5
category: Projects
---

[Poster](https://docs.google.com/presentation/d/1fQuShGARc7tGigU-SwInjhqPtVhAYav6_uwPYCFloDI/edit)

[Code](https://github.com/shrutijain1405/Minitorch-flash-attention)

---

{% include figure.html path="assets/img/projects/flash_attention.png" title="Flash Attention Benchmark Results" class="img-fluid rounded z-depth-1" %}

This project implements and benchmarks Flash-Attention and several of its variants within a custom Vision Transformer built on Minitorch — a from-scratch deep learning framework in Python and CUDA — comparing standard attention, Flash-Attention, block-sparse attention, and multi-query attention across wall-clock time, memory usage, and numerical correctness at varying sequence lengths, batch sizes, and image resolutions to characterize the memory-throughput trade-offs relevant to ViT workloads.