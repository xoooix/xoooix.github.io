---
layout: pagest
title: Paginas
---

### Páginas disponíveis

{% assign pages_list = site.pages %}
<h4>layout page</h4>
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

<h4>layout pagest</h4>
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

<h4>layout default</h4>
<ul>
{% for node in pages_list %}
{% if node.title != null %}
{% if node.layout == "default" %}
<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>
{% endif %}
{% endif %}
{% endfor %}
</ul>

<h4>layout post</h4>
<ul>
{% for node in pages_list %}
{% if node.title != null %}
{% if node.layout == "post" %}
<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>
{% endif %}
{% endif %}
{% endfor %}
</ul>
