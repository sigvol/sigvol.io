---
layout: archive
title: "News"
type: pages
permalink: /news/
author_profile: true
---

{% include base_path %}

{% for post in site.news reversed %}
  {% include archive-single-recent-news.html %}
{% endfor %}