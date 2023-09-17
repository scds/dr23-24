---
layout: home
title: Home
nav_order: 1
---

{%- assign workshops = site.pages | sort: "title" -%}

<img src="assets/img/drslate.png" alt="Workshop Title Slide" width="720">

# 2023-2024 Digital Research Workshops

Work in Progress

## 2023-24 DR Workshop Topics     

<div markdown="1" style="border: 1px solid #7a003c; border-radius: 6px; margin-bottom: 1em; padding: 0.5em 1em 0; margin-top: 1em;" class="toc">
<summary style="cursor:default; display: block; border-bottom: 1px solid #302d36; margin-bottom: 0.5em">
  Workshops
</summary>
<ul>
{% for workshop in workshops %}
    {% if workshop.title != null and workshop.title != "Home" %}
<!-- - [{{workshop.title}}]({{workshop.url}}) -->
<li><a href="{{workshop.url}}">{{workshop.title}}</a></li>
    {% endif %}
{% endfor %}
</ul>
</div>