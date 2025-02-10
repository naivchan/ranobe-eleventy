---
layout: layouts/home.njk
title: Tags
date: 2025-02-09T18:49:00.000Z
permalink: /tags/index.html
eleventyNavigation:
  key: Tags
  order: 5
---

<ul>
  {% for tag in collections.tagList %}
  <li>
    <a href="/tag/{{ tag.title | slug }}/">{{ tag.title }} ({{ tag.count }})</a>
  </li>
  {% endfor %}
</ul>
