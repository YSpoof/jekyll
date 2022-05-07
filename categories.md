---
layout: page
title: Categories
permalink: /categories/
---
<ul>
{% for category in site.categories %}
  <li><h2>{{ category | first }}</h2>
    <ul>
    {% for post in category.last %}
      <li>> <a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
    </ul>
  </li>
{% endfor %}
</ul>