---
title: "A Studious Approach to Semi-Supervised Learning"
collection: publications
category: conferences
paperurl: 'https://arxiv.org/abs/2109.08924'
excerpt: 'an empirical study of distillation based semi-supervised learning to overcome overfitting, and boosting performance of small deployable models.'
venue: 'ICBINB workshop in the NeurIPS 2021 conference.'
date: 2021-09-18
---
The problem of learning from few labeled examples while using large amounts of unlabeled data has been approached by various semi-supervised methods. Although these methods can achieve superior performance, the models are often not deployable due to the large number of parameters. This paper is an ablation study of distillation in a semi-supervised setting, which not just reduces the number of parameters of the model but can achieve this while improving the performance over the baseline supervised model and making it better at generalizing. After the supervised pretraining, the network is used as a teacher model, and a student network is trained over the soft labels that the teacher model generates over the entire unlabeled data. We find that the fewer the labels, the more this approach benefits from a smaller student network. This brings forward the potential of distillation as an effective solution to enhance performance in semi-supervised computer vision tasks while maintaining deployability.
