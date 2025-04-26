---
layout: home
title: "SLK R171 Bordbuch"
subtitle: "Wartungen, Pflege und Upgrades dokumentiert."
author_profile: false
---

Willkommen in meinem Restaurierungstagebuch rund um meinen Mercedes SLK R171 Kompressor!

Hier dokumentiere ich alle durchgeführten Wartungen, Pflegearbeiten und Upgrades.

## Letzte Einträge

{% assign sorted_posts = site.posts | sort: "date" | reverse %}
{% for post in sorted_posts %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})  
  <small>{{ post.date | date: "%d.%m.%Y" }}{% if post.km %}, ca. {{ post.km | number_with_delimiter: delimiter: "." }} km{% endif %}</small>
{% endfor %}
