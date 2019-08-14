---
layout: archive
title: "Posts"
permalink: /posts/
author_profile: false
entries_layout: grid
---

{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}
