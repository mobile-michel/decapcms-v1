---
title: My blog is here
link-name: Blog
description: This blog is about photography.
author: Michel Maillard
date: 2024-01-03
tags: ["primary", "footer"]
---
{% for post in collections.blog %}
- [{{ post.data.title }}]({{ post.url | url }}) published on {{ post.data.date | date: '%d  %b %Y' }} by {{ post.data.author }}
{% endfor %}