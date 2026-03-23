---
title: Inicio
layout: default
---

# Observatorio Crítica Riojana

Análisis independiente de la política local en La Rioja. Datos, tendencias y preguntas que los medios tradicionales evitan.

## Últimas notas

{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
{% for post in sorted_posts limit: 6 %}
<div style="margin-bottom: 2rem;">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p><small>{{ post.date | date: "%d %b %Y" }} • {{ post.categories | join: ", " }}</small></p>
  <p>{{ post.excerpt | strip_html | truncate: 200 }} <a href="{{ post.url }}">Leer más →</a></p>
</div>
{% endfor %}

[Ver todas las notas](/notas) • [RSS feed](/feed.xml)
