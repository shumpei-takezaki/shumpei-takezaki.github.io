---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Shumpei Takezaki (竹崎 隼平 in Japanse), a Ph.D student at Kyushu University under the supervision of Prof. [Seiichi Uhicda](https://human.ait.kyushu-u.ac.jp/~uchida/index-e.html).

Before starting my Ph.D, I received my undergraduate degree in ECE from the Kagoshima Technical College, Kagoshima, JAPAN.

My research is on generative modeling and medical imaging. I am particularly interested in the applications of generative models for medical imaging.

## News
hoge

## Publications
For a more comprehensive list of publications, please visit my [Google Scholar](https://scholar.google.com/citations?user=LaScvbQAAAAJ&hl=en) page.
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}
