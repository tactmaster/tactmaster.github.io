---
layout: default
---
<article class="post">

  <header class="post-header">
    <h1 class="post-title">{{ page.title | escape }}</h1>
  </header>

  <div class="post-content">

<p align="center">

  <img src="{{page.image}}" alt="{{page.name}}" height="200px">
  
</p>
    {{ content }}
  </div>

  <p><a href="https://github.com/tactmaster/tactmaster.github.io/edit/main/{{ page.path }}">✏️ Edit this recipe on GitHub</a></p>

</article>


