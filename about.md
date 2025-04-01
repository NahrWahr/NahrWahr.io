---
layout: page
title: About Me
permalink: /about/
---

<div class="content-card">
  <!-- Optional: Uncomment if you add a profile photo -->
  <!-- <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Your Name" class="profile-image" width="150" height="150"> -->
  
  <h2>Hi, I'm [Your Name]</h2>
  
  <p>[Write a compelling introduction about yourself, your background, and what drives your intellectual curiosity. What questions are you trying to answer through your writing? What perspectives do you bring to your analysis?]</p>
</div>

<div class="content-card">
  <h2>Background & Experience</h2>
  
  <h3>Education</h3>
  <ul>
    <li><strong>[Your Degree]</strong>, [University Name] ([Year])</li>
    <!-- Add more education items as needed -->
  </ul>
  
  <h3>Professional Experience</h3>
  <ul>
    <li>
      <strong>[Job Title]</strong>, [Company Name] ([Years])
      <p>[Brief description of your role and achievements]</p>
    </li>
    <!-- Add more experience items as needed -->
  </ul>
  
  <h3>Key Skills & Areas of Expertise</h3>
  <ul>
    <li>[Skill/Area of Expertise 1]</li>
    <li>[Skill/Area of Expertise 2]</li>
    <li>[Skill/Area of Expertise 3]</li>
    <!-- Add more skills as needed -->
  </ul>
</div>

<div class="content-card">
  <h2>My Approach to Writing & Analysis</h2>
  
  <p>[Describe your methodology, what influences your thinking, and how you approach the topics you write about. What makes your perspective unique or valuable?]</p>
  
  <h3>Areas of Interest</h3>
  <ul>
    <li>[Area of Interest 1]</li>
    <li>[Area of Interest 2]</li>
    <li>[Area of Interest 3]</li>
    <!-- Add more areas as needed -->
  </ul>
</div>

<div class="content-card">
  <h2>Connect With Me</h2>
  
  <p>I'm always interested in thoughtful discussions and new perspectives. Feel free to reach out!</p>
  
  <ul>
    <li><strong>Email:</strong> your.email [at] example.com</li>
    {% if site.github_username %}
    <li><strong>GitHub:</strong> <a href="https://github.com/{{ site.github_username }}" target="_blank">{{ site.github_username }}</a></li>
    {% endif %}
    {% if site.twitter_username %}
    <li><strong>Twitter:</strong> <a href="https://twitter.com/{{ site.twitter_username }}" target="_blank">@{{ site.twitter_username }}</a></li>
    {% endif %}
    {% if site.linkedin_username %}
    <li><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/{{ site.linkedin_username }}" target="_blank">{{ site.linkedin_username }}</a></li>
    {% endif %}
    <!-- Add more contact methods as needed -->
  </ul>
</div>
