---
layout: pagest
title: Arquivo
---

## Índice de Artigos, Posts

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
