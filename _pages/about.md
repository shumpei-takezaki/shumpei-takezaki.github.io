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

## News
- <span style="color:green"> [Paper Acceptance]: </span> [Inverse Scene Text Removal](https://arxiv.org/abs/2506.21002) got accepted to **ICDAR 2025**.
- <span style="color:green"> [Paper Acceptance]: </span> [Self-Relaxed Joint Training: Sample Selection for Severity Estimation with Ordinal Noisy Labels](https://arxiv.org/abs/2410.21885) got accepted to **WACV 2025 Oral**.
- <span style="color:green"> [Paper Acceptance]: </span> [Guidance-base Diffusion Models for Improving Photoacoustic Image Quality](https://arxiv.org/abs/2502.06354) got accepted to **BMVC 2024**.

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
