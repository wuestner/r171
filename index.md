---
layout: home
title: "SLK R171 Restaurierungstagebuch"
subtitle: "Willkommen im Restaurierungstagebuch meines Mercedes SLK R171 Kompressor."
---

## Übersicht

Hier dokumentiere ich Wartungen, Pflege und Upgrades rund um meinen Mercedes SLK R171. 

## Wartungshistorie

Hier erscheinen alle Wartungseinträge chronologisch.

{% for post in site.posts %}
### [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
> {{ post.excerpt }}
{% endfor %}
