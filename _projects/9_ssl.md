---
layout: page
title: Knowledge Distillation for Learning with Limited Labels
description: Student-model capacity and generalization under limited supervision · NeurIPS 2021 workshop
img: assets/img/projects/ssl.png
importance: 9
category: Projects
---

**Venue:** ICBINB Workshop — NeurIPS 2021

[Paper](https://arxiv.org/abs/2109.08924)

<!-- [PDF](https://arxiv.org/pdf/2109.08924) -->

---

{% include figure.html path="assets/img/projects/ssl.png" title="Semi-Supervised Distillation" class="img-fluid rounded z-depth-1" %}

This study examines knowledge distillation when labeled data is scarce but unlabeled examples are available. A supervised teacher generates soft labels for training smaller student networks, and ablations investigate how model capacity interacts with label availability.

The experiments show that smaller students can improve over the supervised baseline in the evaluated settings, connecting data-efficient learning with compact model design.
