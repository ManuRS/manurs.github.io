---
title: Manuel Reyes Sánchez - Blog
description: "Mi blog personal"
layout: future
special_header: true
---

<!-- La plantilla carga custom.css -->

<picture>
  <source media="(max-width: 42em)" srcset="{{ '/resources/banner_web_phone.png' | relative_url }}">
  <source media="(min-width: 42em)" srcset="{{ '/resources/banner_web_desktop.png' | relative_url }}">
  <img src="{{ '/resources/banner_web_phone.png' | relative_url }}" alt="Banner">
</picture>

<a class="btnmenu" href="/">Home</a> | 

<h2 style="margin-top: 1rem;"> Blog </h2>

**Mi espacio personal para compartir textos**

<picture>
  <source media="(min-width: 42em)" srcset="{{ '/img/blog_desktop_1.webp' | relative_url }}" width="1200">
  <img src="{{ '/img/blog_phone_1.webp' | relative_url }}" alt="Foto" style="padding-right: 0px; padding-left: 0px;">
</picture>

{% for post in site.posts %}

### **<a href="{{ post.url }}">{{ post.title }}</a>**

{{ post.subtitle }}

*{{ post.fecha }}*

{% endfor %}
