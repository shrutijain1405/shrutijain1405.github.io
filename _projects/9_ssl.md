---
layout: page
title: A Studious Approach to Semi-Supervised Learning
description: NeurIPS 2021 Workshop
img: assets/img/projects/ssl.png
importance: 9
category: Research
---

**Venue:** Workshop — NeurIPS 2021

**Links:** [Paper](https://arxiv.org/abs/2109.08924) &nbsp;|&nbsp; [PDF](https://arxiv.org/pdf/2109.08924)

---

## Overview

The availability of large quantities of unlabeled data alongside limited labeled examples is a common and practically important setting in computer vision. Semi-supervised learning methods aim to exploit unlabeled data to improve model performance beyond what is achievable with labeled data alone. However, a persistent tension exists between achieving high accuracy and maintaining a model footprint small enough for real-world deployment.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/projects/ssl.png" title="Semi-Supervised Distillation" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Knowledge distillation in a semi-supervised setting: a teacher network trained on labeled data generates soft labels over unlabeled data to train a compact student network.
</div>

## Approach

This paper presents an ablation study of **knowledge distillation in a semi-supervised setting**, exploring how distillation can simultaneously reduce model size and improve generalization over a baseline supervised model. The approach proceeds in two stages:

1. **Supervised Pretraining:** A larger teacher network is trained on the available labeled examples.
2. **Semi-Supervised Distillation:** The teacher generates soft probability labels over the full unlabeled dataset. A smaller student network is then trained on these soft labels, leveraging the unlabeled data as a source of additional supervision.

A key finding is that **the fewer the labeled examples available, the more benefit is gained from using a smaller student network** — suggesting that distillation is especially valuable in very low-label regimes, where model capacity would otherwise lead to overfitting.

## Key Contributions

- Systematic ablation study of knowledge distillation in semi-supervised computer vision
- Demonstration that distillation improves both accuracy and deployability over the supervised baseline
- Evidence that smaller student networks benefit more in lower-label regimes
- Insights into distillation as an effective and practical tool for semi-supervised learning