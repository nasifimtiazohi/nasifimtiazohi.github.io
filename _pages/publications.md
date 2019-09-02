---
layout: page
permalink: /publications/
title: publications
description: A list containing most of my recent publications.
type: ["Full Conference Paper" ,"Short Conference Paper","Workshop Paper","Poster" ]
---

{% for y in page.type %}
  <h3>{{y}}</h3>
  {% bibliography -f papers -q @*[papertype={{y}}]* %}
{% endfor %}