---
layout: home
title: "SLK R171 Bordbuch"
subtitle: "Wartungen, Pflege und Upgrades dokumentiert."
author_profile: false
---
<style>
  table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 2rem;
  }
  th, td {
    border: 1px solid #ddd;
    padding: 8px;
    text-align: center;
  }
  th {
    background-color: #f2f2f2;
  }
  tr:hover {
    background-color: #f9f9f9;
  }
</style>

Willkommen in meinem Bordbuch rund um meinen Mercedes SLK R171 Kompressor!

Hier dokumentiere ich alle durchgeführten Wartungen, Pflegearbeiten und Upgrades.

## Wartungshistorie

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
