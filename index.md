---
layout: home
title: Welcome
---

<div class="content-card">
  <h2>Hi, I'm [Your Name]</h2>
  
  <p>Welcome to my digital garden of thoughts and ideas. This is where I explore topics related to <strong>[your key interests]</strong> through essays, analysis, and reflections.</p>
  
  <p>My goal is to share insights from my reading and research, fostering thoughtful discussion and deeper understanding of the subjects that fascinate me.</p>
</div>

<div class="homepage-navigation">
  <p>Explore what I've been working on:</p>
  
  <a href="{{ '/work/' | relative_url }}" class="button">Essays & Analyses</a>
  <a href="{{ '/about/' | relative_url }}" class="button">About Me</a>
  <!-- Add more navigation buttons as needed -->
</div>

## Recent Writing
<div class="post-preview-container">
{% for post in site.posts limit:3 %}
  <div class="content-card">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: site.date_format }}</p>
    
    {% if post.excerpt %}
      <div class="post-excerpt">
        {{ post.excerpt }}
      </div>
    {% endif %}
    
    <a href="{{ post.url | relative_url }}" class="read-more-link">Continue reading →</a>
    
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
  </div>
{% endfor %}
</div>

{% if site.posts.size > 3 %}
<div style="text-align: center; margin-top: 2em;">
  <a href="{{ '/work/' | relative_url }}" class="button">View All Posts</a>
</div>
{% endif %}
