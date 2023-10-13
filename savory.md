---
layout: page
permalink: /savory/
title: Savory
---

{% for savory in site.savory %}
| ![savory.name]( {{savory.image}} ){:height="40px" } | [ {{savory.name}} ]( {{ savory.url }}) | {% endfor %}
