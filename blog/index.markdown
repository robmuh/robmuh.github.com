---
layout: blog
---

This is my blog, blah blah

{% for post in site.posts %}
  {% include blog_post.html %}
{% endfor %}
