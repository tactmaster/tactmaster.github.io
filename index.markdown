---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---


# Recipes
{% for page in site.pages %}
  {% if page.categories contains 'recipe' %}
  [ {{page.title}} ]( {{ page.url }} )
  {% endif %}
{% endfor %}

