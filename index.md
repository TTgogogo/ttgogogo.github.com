---
layout: page
title: Explore the world!
tagline: 霓棠烟鱼的blog
---
{% include JB/setup %}

   
<ul class="posts">
  {% for post in site.posts %}
    <li><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a><p>{{ post.content | split:'<!--more-->' |first }}</p></li>
  {% endfor %}
</ul>