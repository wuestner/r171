---
layout: home
title: "SLK R171 Bordbuch"
subtitle: "Wartungen, Pflege und Upgrades dokumentiert."
author_profile: false
---

Willkommen in meinem Restaurierungstagebuch rund um meinen Mercedes SLK R171 Kompressor!

Hier dokumentiere ich alle durchgeführten Wartungen, Pflegearbeiten und Upgrades.

<table>
  <thead>
    <tr>
      <th>Datum</th>
      <th>Wartung</th>
      <th>Kilometerstand</th>
    </tr>
  </thead>
  <tbody>
    {% assign sorted_posts = site.posts | sort: "date" %}
    {% for post in sorted_posts %}
    <tr>
      <td>{{ post.date | date: "%d.%m.%Y" }}</td>
      <td><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></td>
      <td>{% if post.km %}ca. {{ post.km | number_with_delimiter: delimiter: "." }} km{% else %}-{% endif %}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
