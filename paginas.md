---
layout: pagest
title: Paginas
---

### Páginas disponíveis

{% assign pages_list = site.pages %}
####layout page
<ul>
{% for node in pages_list %}
{% if node.title != null %}
{% if node.layout == "page" %}
<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>
{% endif %}
{% endif %}
{% endfor %}
</ul>
####layout pagest
<ul>
{% for node in pages_list %}
{% if node.title != null %}
{% if node.layout == "pagest" %}
<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>
{% endif %}
{% endif %}
{% endfor %}
</ul>
