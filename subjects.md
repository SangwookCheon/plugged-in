---
layout: articles
title: Subjects
show_title: false
articles:
  data_source: site.subjects
  type: grid
---

{% for item in site.subjects %}
  <h2>
    <a href="{{ item.url }}">
      {{ item.content }}
    </a>
  </h2>
  <p>{{ item.content | markdownify }}</p>
{% endfor %}
