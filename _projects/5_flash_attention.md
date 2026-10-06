---
layout: page
title: Efficient Attention for Vision Transformers
description: Python/CUDA implementation and evaluation of memory, runtime, and numerical correctness
img: assets/img/projects/flash_attention.png
importance: 5
category: Projects
---

[Poster](https://docs.google.com/presentation/d/1fQuShGARc7tGigU-SwInjhqPtVhAYav6_uwPYCFloDI/edit)

[Code](https://github.com/shrutijain1405/Minitorch-flash-attention)

---

{% include figure.html path="assets/img/projects/flash_attention.png" title="Flash Attention Benchmark Results" class="img-fluid rounded z-depth-1" %}

This project implements and benchmarks attention mechanisms within a custom Vision Transformer built on **Minitorch**, a deep learning framework in Python and CUDA. It compares **standard, Flash, block-sparse, and multi-query attention** across sequence lengths, batch sizes, and image resolutions.

The evaluation measures wall-clock time, memory use, and numerical correctness to characterize the tradeoffs involved in efficient vision-model execution.
