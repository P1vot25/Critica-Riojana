---
title: Inicio
layout: home               # o default si no tenés custom
nav_order: 1
---

# Observatorio Crítica Riojana

Análisis independiente de la política local.  
Últimas notas ↓

{% for post in site.posts limit: 5 %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%d %b %Y" }}
{% endfor %}

[RSS feed](/feed.xml) para seguir actualizaciones.
