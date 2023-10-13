---
layout: page
permalink: /sweet/
title: Sweet
---

{% for sweet in site.sweet %}
| ![sweet.name]( {{sweet.image}} ){:height="40px" } | [ {{sweet.name}} ]( {{ sweet.url }}) | {% endfor %}