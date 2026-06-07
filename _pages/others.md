---
title: ""
permalink: /others/
author_profile: true
---

## Awards
{% for item in site.data.others.awards %}
* {{ item.text }}
{% endfor %}

## Grants
{% for item in site.data.others.grants %}
* {{ item.text }}
{% endfor %}
