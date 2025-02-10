---
layout: layouts/home.njk
title: Tags
date: 2025-02-09T18:49:00.000Z
permalink: /tags/index.html
eleventyNavigation:
  key: Tags
  order: 5
---
{% for post in collections[tag] %}
<div class="py-4 sm:py-10">
  <p>
    <span class="text-2xl sm:text-4xl font-bold hover:underline"><a href="{{ post.url }}">{{ post.data.title }}</a></span>
  </p>
  <em>{{ post.date | date: "%Y-%m-%d" }}</em>
  <p class="mt-4">{{ post.data.post_excerpt }}... 
    <span class="hover:underline text-indigo-500"><a href="{{ post.url }}">Read More</a></span>
  </p>
</div>
{% endfor %}
