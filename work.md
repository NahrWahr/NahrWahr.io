---
layout: page
title: My Writing
permalink: /work/
---

<div class="content-card">
  <p>Here you'll find my analyses, essays, and reflections. I regularly post thoughts on chapters and articles I read, as well as longer-form pieces exploring topics I'm passionate about.</p>
</div>

## Latest Posts

<div class="post-list-container">
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h3 class="post-link">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <span class="post-date">{{ post.date | date: site.date_format }}</span>
        
        {% if post.excerpt %}
          <div class="post-excerpt">
            {{ post.excerpt }}
            <a href="{{ post.url | relative_url }}" class="read-more-link">Continue reading →</a>
          </div>
        {% endif %}
        
        {% if post.categories.size > 0 or post.tags.size > 0 %}
        <div class="post-metadata">
          {% if post.categories.size > 0 %}
          <div class="post-categories">
            <span>Categories:</span>
            {% for category in post.categories %}
              <a class="category-item" href="{{ '/categories/#' | append: category | relative_url }}">{{ category }}</a>
            {% endfor %}
          </div>
          {% endif %}
          
          {% if post.tags.size > 0 %}
          <div class="post-tags">
            <span>Tags:</span>
            {% for tag in post.tags %}
              <a class="tag-item" href="{{ '/tags/#' | append: tag | relative_url }}">{{ tag }}</a>
            {% endfor %}
          </div>
          {% endif %}
        </div>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
</div>
