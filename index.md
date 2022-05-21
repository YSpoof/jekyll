---
title: Home
layout: home
---

<h2>Posts:</h2>
<ul id="posts">
{% for post in site.posts %}
<li class="post"><a href="{{post.url | relative_url }}">{{post.title}}</a></li>
{% endfor %}
</ul>
