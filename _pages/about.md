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
  .news-row { display: flex; gap: 1.2em; padding: 0.5em 0; border-top: 1px solid var(--line-color); }
  .news-row.first { border-top: none; }
  .news-more { background: none; border: none; padding: 0.5em 0; color: var(--global-link-color); cursor: pointer; font: inherit; }
  .news-more:hover { text-decoration: underline; }
  .news-date { flex: 0 0 5.5em; color: gray; white-space: nowrap; }
  .news-text { flex: 1; }
  @media (max-width: 480px) { .news-row { flex-direction: column; gap: 0.1em; } }
  .contact-box { background: var(--box-bg); border-radius: 0.75rem; padding: 1.2em 1.5em; font-size: 0.85em; line-height: 1.7; color: var(--box-text); }
  .contact-box p { margin: 0; }
  .contact-org { font-weight: 600; color: var(--accent-color); margin-bottom: 0.3em !important; }
  .contact-mail { margin-top: 0.6em !important; }
  .contact-mail span { font-family: monospace; color: var(--global-link-color); }
</style>

## News
{% assign news_visible = 5 %}{% assign news_split = news_visible | plus: 1 %}
<div class="news-list">
{% for item in site.data.news %}{% if forloop.index == news_split %}<div id="news-extra" hidden>{% endif %}<div class="news-row{% if forloop.first %} first{% endif %}"><div class="news-date">{{ item.date }}</div><div class="news-text" markdown="span">{{ item.text }}</div></div>
{% endfor %}{% if site.data.news.size > news_visible %}</div>
<button type="button" class="news-more" id="news-toggle" aria-expanded="false">Show more</button>
<script>
  document.getElementById('news-toggle').addEventListener('click', function () {
    var extra = document.getElementById('news-extra');
    var open = extra.hidden;
    extra.hidden = !open;
    this.textContent = open ? 'Show less' : 'Show more';
    this.setAttribute('aria-expanded', open);
  });
</script>{% endif %}</div>

## Publications
For a more comprehensive list of publications, please see [Publications](/publications/) or visit [Google Scholar](https://scholar.google.com/citations?user=TJHgmY8AAAAJ&hl=en) page.

## Contact
<div class="contact-box">
  <p class="contact-org">Human Interface Laboratory, Department of Advanced Information Technology</p>
  <p>Kyushu University</p>
  <p>744, Motooka, Nishi-ku, Fukuoka-shi, 819-0395 JAPAN</p>
  <p>TEL: +81-92-802-3574</p>
  <p class="contact-mail">E-mail: <span>shumpei.takezaki[at]human.ait.kyushu-u.ac.jp</span></p>
</div>
