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

<style>
  .news-row { display: flex; gap: 1.2em; padding: 0.5em 0; border-bottom: 1px solid #ddd; }
  .news-row:last-child { border-bottom: none; }
  .news-date { flex: 0 0 5.5em; color: gray; white-space: nowrap; }
  .news-text { flex: 1; }
  @media (max-width: 480px) { .news-row { flex-direction: column; gap: 0.1em; } }
  .contact-list ul { list-style: none !important; padding-left: 0; }
  .contact-list li { list-style: none !important; }
</style>

## News
<div class="news-list">
{% for item in site.data.news %}<div class="news-row"><div class="news-date">{{ item.date }}</div><div class="news-text" markdown="span">{% if item.link and item.link != "" %}[{{ item.title }}]({{ item.link }}){% else %}{{ item.title }}{% endif %} {{ item.description }}</div></div>
{% endfor %}</div>

## Publications
For a more comprehensive list of publications, please see [Publications](/publications/) or visit [Google Scholar](https://scholar.google.com/citations?user=TJHgmY8AAAAJ&hl=en) page.

## Contact
<div class="contact-list" markdown="1">
- Address: Human Interface Laboratory, Department of Advanced Information Technology, Kyushu University. 744, Motooka, Nishi-ku, Fukuoka-shi, 819-0395 JAPAN
- TEL: +81-92-802-3574
- E-mail: shumpei.takezaki[at]human.ait.kyushu-u.ac.jp

</div>
