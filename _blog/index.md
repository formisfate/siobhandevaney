---
layout: default
title: "📝 Blog"
has_children: true
permalink: /blog/
nav_order: 4
hidden: true
---

# 📝 Blog

Occasional thoughts, fragments, and full-form writing experiments.

{% for post in site.blog %}
  {% unless post.name == "index" %}
- [{{ post.title }}]({{ post.url | relative_url }})
  {% endunless %}
{% endfor %}
