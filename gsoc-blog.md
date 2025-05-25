---
layout: archive
title: "My Google Summer of Code (GSoC 2025) Journey"
permalink: /gsoc-blog/
author_profile: true
---

I'm participating in Google Summer of Code 2025 working on the project titled ["**Using Data-Driven, Physics-Informed Machine Learning to Model Fluid Properties in Computational Fluid Dynamics**"](https://summerofcode.withgoogle.com/programs/2025/projects/iFt1m8Wx) with the organization **Stitching SU2**. This page chronicles my weekly progress, challenges, and learnings throughout the program.

## About My Project
This project proposes to enhance SU2’s CFD capabilities by optimizing the MLPCpp Neural Network module in the Non-Ideal Compressible Fluid Dynamics framework through performance improvements and better inverse regression, delivered via a tutorial and a code update with benchmarks.

## Weekly Blog Posts
{% assign gsoc_posts = site.posts | where_exp: "post", "post.categories contains 'GSoC'" %}
{% for post in gsoc_posts %}
  {% include archive-single.html %}
{% endfor %}
