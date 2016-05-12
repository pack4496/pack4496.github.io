---
layout: page
title: All posts
permalink: /posts/
---

{% for post in site.posts %}

[{{ post.title }}]({{ post.url }})

{% endfor %}