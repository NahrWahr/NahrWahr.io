---
layout: page
title: Tags
permalink: /tags/
---

<div class="content-card">
  <p>Browse posts by tag to find content on specific subjects and themes.</p>
</div>

{% assign tags = site.tags | sort %}
<div class="content-card">
  <h2>All Tags</h2>
  <div class="tags-list">
    {% for tag in tags %}
      <a href="#{{ tag[0] }}" class="tag-item">{{ tag[0] }}</a>
    {% endfor %}
  </div>
</div>

{% for tag in tags %}
  <div class="content-card">
    <h2 id="{{ tag[0] }}">{{ tag[0] }}</h2>
    <ul class="post-list">
      {% for post in tag[1] %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          <span class="post-date">{{ post.date | date: site.date_format }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
