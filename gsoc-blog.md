---
layout: archive
title: "My Google Summer of Code Journey"
permalink: /gsoc-blog/
author_profile: true
---

I'm participating in Google Summer of Code 2025 working on [Project Name] with [Organization Name]. This page chronicles my weekly progress, challenges, and learnings throughout the program.

## About My Project
Brief description of what your GSoC project involves and what you hope to achieve.

## Weekly Blog Posts

{% assign gsoc_posts = site.posts | where_exp: "post", "post.categories contains 'GSoC'" %}
{% for post in gsoc_posts %}
  {% include archive-single.html %}
{% endfor %}
