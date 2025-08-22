---
layout: default
title: "Recipes"
---

# Recipes

<ul>
{% for recipe in site.recipes %}
  <li><a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.title | default: recipe.name | remove: ".md" }}</a></li>
{% endfor %}
</ul>