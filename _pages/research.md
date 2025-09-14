---
permalink: /research/
title: "Research"
layout: single
---

Here you can find my working papers, published articles, and ongoing projects.

<ul>
{% for paper in site.research %}
  <li>
    <strong><a href="{{ paper.url | relative_url }}">{{ paper.title }}</a></strong><br>
    {{ paper.content | strip_html | truncate: 200 }}<br>
    {% if paper.pdf %}
      <a href="{{ paper.pdf | relative_url }}">Download PDF</a>
    {% endif %}
  </li>
{% endfor %}
</ul>
