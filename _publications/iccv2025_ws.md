---
title: "NoiseCutMix: A Novel Data Augmentation Approach by Mixing Estimated Noise in Diffusion Models"
collection: publications
category: conferences
permalink: /publication/iccv2025_ws
excerpt: ''
status: 'Published'
venue: 'ICCV 2025 Workshop'
authors: '<strong> Shumpei Takezaki</strong>, Ryoma Bise, Shinnosuke Matsuo'
paperurl: https://arxiv.org/abs/2509.00378
code: https://github.com/shumpei-takezaki/NoiseCutMix
date: 2025-08-29
---

![](../images/iccv2025_ws_overview.png)

> In this study, we propose a novel data augmentation method that introduces the concept of CutMix into the generation process of diffusion models, thereby exploiting both the ability of diffusion models to generate natural and high-resolution images and the characteristic of CutMix, which combines features from two classes to create diverse augmented data. Representative data augmentation methods for combining images from multiple classes include CutMix and MixUp. However, techniques like CutMix often result in unnatural boundaries between the two images due to contextual differences. Therefore, in this study, we propose a method, called NoiseCutMix, to achieve natural, high-resolution image generation featuring the fused characteristics of two classes by partially combining the estimated noise corresponding to two different classes in a diffusion model. In the classification experiments, we verified the effectiveness of the proposed method by comparing it with conventional data augmentation techniques that combine multiple classes, random image generation using Stable Diffusion, and combinations of these methods.

Please read the [paper](https://arxiv.org/abs/2509.00378) for more details.