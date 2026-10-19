---
title: ""
permalink: /others/
author_profile: true
---

<style>
  .others-list { padding-left: 1.6em; margin: 0 0 1em; font-size: 0.85em; }
  .others-list li { margin: 0; padding: 0.5em 0; border-bottom: 1px solid var(--line-color); line-height: 1.45; }
  .others-list li:last-child { border-bottom: none; }
</style>

## Awards
<ol class="others-list">
{% for item in site.data.others.awards %}<li markdown="span">{{ item.text }}</li>
{% endfor %}</ol>

## Grants
<ol class="others-list">
{% for item in site.data.others.grants %}<li markdown="span">{{ item.text }}</li>
{% endfor %}</ol>
