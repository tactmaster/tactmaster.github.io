---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: All

---

### Sweet

{% for sweet in site.sweet %}
| ![sweet.name]( {{sweet.image}} ){:height="40px" } | [ {{sweet.name}} ]( {{ sweet.url }}) | {% endfor %}

### Savory

{% for savory in site.savory %}
| ![savory.name]( {{savory.image}} ){:height="40px" } | [ {{savory.name}} ]( {{ savory.url }}) | {% endfor %}
