---
layout: page
title: Categories
permalink: /categories/
---

<div class="content-card">
  <p>Browse posts by category to find content related to specific topics.</p>
</div>

{% assign sorted_categories = site.categories | sort %}
{% for category in sorted_categories %}
  <div class="content-card">
    <h2 id="{{ category[0] }}">{{ category[0] }}</h2>
    <ul class="post-list">
      {% for post in category[1] %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          <span class="post-date">{{ post.date | date: site.date_format }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
