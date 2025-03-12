---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Biography
<style>
  a {
    text-decoration: none;
  }
</style>
I am Shumpei Takezaki (竹崎 隼平 in Japanse), a Ph.D student at Kyushu University, Fukuoka, JAPAN, under the supervision of [Prof. Seiichi Uhicda](https://human.ait.kyushu-u.ac.jp/~uchida/index-e.html).

Before starting my Ph.D, I received my undergraduate degree in ECE from the Kagoshima Technical College, Kagoshima, JAPAN.

My research is on generative modeling. I am particularly interested in the applications of generative modeling for medical imaging.

## News
- <span style="color:green"> [Paper Acceptance]: </span> [Self-Relaxed Joint Training: Sample Selection for Severity Estimation with Ordinal Noisy Labels](https://arxiv.org/abs/2410.21885) got accepted to **WACV 2025 Oral**.
- <span style="color:green"> [Paper Acceptance]: </span> [Guidance-base Diffusion Models for Improving Photoacoustic Image Quality](https://arxiv.org/abs/2502.06354) got accepted to **BMVC 2024**.
- <span style="color:green"> [Paper Acceptance]: </span> [Cross-Domain Image Conversion by CycleDM](https://arxiv.org/abs/2403.02919) got accepted to **ICDAR 2024**.

## Recent Publications
For a more comprehensive list of publications, please see [Publications](/publications/) or visit [Google Scholar](https://scholar.google.com/citations?user=TJHgmY8AAAAJ&hl=en) page.
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted limit:3 %}
  {% include archive-single.html %}
{% endfor %}

## Contact
- Address: Human Interface Laboratory, Department of Advanced Information Technology, Kyushu University. 744, Motooka, Nishi-ku, Fukuoka-shi, 819-0395 JAPAN
- TEL: +81-92-802-3574
- E-mail: shumpei.takezaki[at]human.ait.kyushu-u.ac.jp
