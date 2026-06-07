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
{% for item in site.data.news %}
- {% if item.type == "reward" %}<span style="color:red"> [Reward]: </span>{% elsif item.type == "acceptance" %}<span style="color:green"> [Paper Acceptance]: </span>{% endif %}{% if item.link and item.link != "" %}[{{ item.title }}]({{ item.link }}){% else %}{{ item.title }}{% endif %} {{ item.description }}
{% endfor %}

## Publications
For a more comprehensive list of publications, please see [Publications](/publications/) or visit [Google Scholar](https://scholar.google.com/citations?user=TJHgmY8AAAAJ&hl=en) page.

## Contact
- Address: Human Interface Laboratory, Department of Advanced Information Technology, Kyushu University. 744, Motooka, Nishi-ku, Fukuoka-shi, 819-0395 JAPAN
- TEL: +81-92-802-3574
- E-mail: shumpei.takezaki[at]human.ait.kyushu-u.ac.jp
