---
layout: page
permalink: /quotidien/
title: quotidien
description: short daily chatter on random themes
---

<ul class="post-list">
{% for poem in site.quotidien reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
