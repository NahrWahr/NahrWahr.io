---
layout: page
title: Welcome! # You can customize the title
permalink: / # Makes this the root page (homepage)
---

Welcome to my personal website!

This site serves as a central hub for my thoughts, analyses, and essays. I explore topics related to **[mention your key areas of interest, e.g., literature, technology, philosophy, etc.]**.

<!-- Add a container for the buttons for easier styling if needed -->
<div class="homepage-navigation" style="text-align: center; margin: 2em 0;"> {# Optional inline style for centering, or use the class in style.scss #}
  <p style="margin-bottom: 1em;">Explore the main sections:</p> {# Optional text before buttons #}

  <a href="{{ '/work/' | relative_url }}" class="button">View My Work & Essays</a>
  <a href="{{ '/about/' | relative_url }}" class="button">About Me</a>

  {# Add more buttons here if you create more top-level pages later #}
  {# Example: <a href="/projects/" class="button">Projects</a> #}
</div>

My goal is to share insights gained from reading and research, fostering discussion and deeper understanding.

Feel free to explore. You can find my contact details on the [About Me]({{ '/about/' | relative_url }}) page.
