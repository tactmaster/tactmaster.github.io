---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% for recipe in site.recipes %}
| ![recipe.name]( {{recipe.image}} ){:height="40px" } | [ {{recipe.name}} ]( {{ recipe.url }}) | {% endfor %}
