---
layout: page
title: Culture
permalink: /work-culture/
---
<ul>
{% for post in site.posts %}
  {% if post.categories contains "culture" %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endif %}
{% endfor %}
</ul>