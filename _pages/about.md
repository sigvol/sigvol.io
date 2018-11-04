---
permalink: /
title: "About Me"
excerpt: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I am a Ph.D candidate in [Electrical and Computer Engineering](https://www.ee.ucla.edu/) 
, [University of California, Los Angeles](http://www.ucla.edu/). I am a member of
 [Medical Image Informatics Lab](https://www.mii.ucla.edu/), advised by [Prof. Corey Arnold](https://www.mii.ucla.edu/people/cwarnold/)
 and co-advised by [Prof. Greg Pottie](http://www.seas.ucla.edu/~pottie/). My research interests lie in the
 __real-life application of machine learning, especially for healthcare__.

## Recent News
{% include base_path %}
{% for post in site.news reversed %}
  {% include front-recent-news.html %}
  {% if forloop.index == 3 %}
    {% break %}
  {% endif %}
{% endfor %}
[Read more news]({{site.url}}/news)