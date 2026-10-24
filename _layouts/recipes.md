---
layout: default
---
<article class="post">

  <header class="post-header">
    <h1 class="post-title">{{ page.title | escape }} <a href="https://github.com/tactmaster/tactmaster.github.io/edit/main/{{ page.path }}" title="Edit this recipe on GitHub" style="font-size: 0.5em; text-decoration: none; vertical-align: middle;">✏️</a></h1>
  </header>

  <div class="post-content">

<p align="center">

  <img src="{{page.image}}" alt="{{page.name}}" height="200px">
  
</p>
    {{ content }}
  </div>

</article>


