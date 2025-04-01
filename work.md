---
layout: page
title: Work
permalink: /work/
---

Here you'll find my analyses, essays, and reflections. I regularly post thoughts on chapters and articles I read, as well as longer-form pieces.

## Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
      <!-- Optional: Add excerpt -->
      <!-- {{ post.excerpt }} -->
    </li>
  {% endfor %}
</ul>

<!-- You can add more static content here if needed -->
