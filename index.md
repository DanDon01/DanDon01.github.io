---
layout: default
title: Welcome to DanDon01's Blog
---

# Welcome to My GitHub Blog! 

Here’s the latest update:

{% for post in site.posts limit:1 %}
## [{{ post.title }}]({{ post.url }})
**{{ post.date | date: "%B %d, %Y" }}**  
{{ post.excerpt }}
{% endfor %}

---

[View All Posts →](archive)
