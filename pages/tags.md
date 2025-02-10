---
layout: layouts/home.njk
title: Tags
date: 2025-02-09T18:49:00.000Z
permalink: /tags/index.html
eleventyNavigation:
  key: Tags
  order: 5
---
{% for tag in collections.tagList %}

<span>
    <a href="/tags/{{ tag }}"><button class="bg-white hover:bg-gray-100 text-gray-800 font-semibold py-2 px-4 border border-gray-400 rounded shadow mr-6 mb-4">
        {{ tag }}
    </button>
    </a>
</span>
{% endfor %}
