---
layout: default
title: Welcome to My Blog
---

<div style="text-align: center; margin-bottom: 2rem;">
  <pre style="font-size: 1rem; line-height: 1.2; color: #bd93f9;">
      __        __   _                            _     
      \ \      / /__| | ___ ___  _ __ ___   ___  | |___ 
       \ \ /\ / / _ \ |/ __/ _ \| '_ ` _ \ / _ \ | / __|
        \ V  V /  __/ | (_| (_) | | | | | |  __/ | \__ \
         \_/\_/ \___|_|\___\___/|_| |_| |_|\___|_|_|___/
  </pre>
  <h1 style="font-size: 2.5rem; font-weight: bold; margin-bottom: 0.5rem; color: #bd93f9;">
    Welcome to My Tech Blog
  </h1>
  <p style="font-size: 1.2rem; color: #b3b3b3;">
    Sharing my projects, coding adventures, and everything I learn along the way.
  </p>
</div>

<hr style="border: 0; height: 1px; background: #555; margin-bottom: 2rem;">

<div style="text-align: left;">
  <h2 style="font-size: 2rem; color: #bd93f9;">Latest Blog Post</h2>

  {% for post in site.posts limit:1 %}
    <div style="border-left: 5px solid #bd93f9; padding-left: 1rem; margin-bottom: 1rem;">
      <h3 style="font-size: 1.5rem;">
        <a href="{{ post.url }}" style="color: #bd93f9; text-decoration: none;">
          {{ post.title }}
        </a>
      </h3>
      <p style="color: #b3b3b3; font-size: 0.9rem;">
        <strong>{{ post.date | date: "%B %d, %Y" }}</strong>
      </p>
      <p>{{ post.excerpt }}</p>
    </div>
  {% endfor %}

  <a href="/archive" style="display: inline-block; margin-top: 1rem; font-size: 1rem; color: #8be9fd; text-decoration: none; border-bottom: 1px solid #8be9fd;">
    View All Posts →
  </a>
</div>
