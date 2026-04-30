---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Biography
I am Shumpei Takezaki (竹崎 隼平 in Japanse), a Ph.D student at Kyushu University, Fukuoka, JAPAN, under the supervision of [Prof. Seiichi Uhicda](https://human.ait.kyushu-u.ac.jp/~uchida/index-e.html).

Before starting my Ph.D, I received my undergraduate degree in ECE from the Kagoshima Technical College, Kagoshima, JAPAN.

My research is on generative modeling. I am particularly interested in the applications of generative modeling for medical imaging.

## Recent News
- <span style="color:red"> [Reward]: </span> [Bridging the Density Gap: Diffusion Model for Stepwise Generation of Dense Cell Images from Sparse Data]() got **ISBI 2026 Best Paper Award-Runner UP** (Top 3 papers selected for publication).
- <span style="color:green"> [Paper Acceptance]: </span> [Cell Instance Segmentation via Multi-Task Image-to-Image Schrödinger Bridge](https://arxiv.org/abs/2604.12318) got accepted to **IJCNN 2026**.
- <span style="color:green"> [Paper Acceptance]: </span> [SCoRe: Clean Image Generation from Diffusion Models Trained on Noisy Images](https://arxiv.org/abs/2604.09436) got accepted to **IJCNN 2026**.

## Publications
For a more comprehensive list of publications, please see [Publications](/publications/) or visit [Google Scholar](https://scholar.google.com/citations?user=TJHgmY8AAAAJ&hl=en) page.

{% assign sorted = site.publications | reverse %}
{% assign count = 0 %}
{% for post in sorted %}
  {% assign category = post.category | downcase %}
  {% if category == "conferences" or category == "journals" %}
    {% include archive-single.html post=post %}
    {% assign count = count | plus: 1 %}
  {% endif %}
  {% if count == 3 %}
    {% break %}
  {% endif %}
{% endfor %}

## Contact
- Address: Human Interface Laboratory, Department of Advanced Information Technology, Kyushu University. 744, Motooka, Nishi-ku, Fukuoka-shi, 819-0395 JAPAN
- TEL: +81-92-802-3574
- E-mail: shumpei.takezaki[at]human.ait.kyushu-u.ac.jp
